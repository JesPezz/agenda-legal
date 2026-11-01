# Formulario «Seguridad de los datos» de Google Play — respuestas sugeridas

Paquete: `com.jespezz.agenda_movil` · Versión a publicar: 15.3+

## 1. Recopilación y uso

- **¿Tu app recopila o comparte datos de usuario requeridos?** → **Sí, pero solo si el usuario conecta Google Drive** (función opcional). Sin conexión, la app no transmite nada.
- **¿Los datos se cifran en tránsito?** → **Sí** (TLS).
- **¿El usuario puede solicitar la eliminación de sus datos?** → **Sí** (desde la app con «Borrar base», borrando el archivo en su Drive, o con el **borrado a distancia** desde otro equipo vinculado a la misma copia).
- **¿Los datos se procesan de forma efímera?** → **Sí** para el cálculo de reportes (no se almacena nada fuera del equipo).

## 2. Tipos de datos (marcar)

| Categoría | Tipo | Recopilado | Compartido | Finalidad | Opcional |
|---|---|---|---|---|---|
| Información personal | Nombre | Sí | No | Funcionalidad de la app | Sí (solo con Drive) |
| Información personal | Otra información (CURP, fecha de nacimiento, sexo, matrícula, teléfono y dirección de tutores) | Sí | No | Funcionalidad de la app | Sí |
| Información educativa | Calificaciones, asistencia, evaluaciones | Sí | No | Funcionalidad de la app | Sí |
| Archivos y documentos | Documentos generados (Word/PDF) y copia de la base | Sí | No | Funcionalidad de la app | Sí |

> **Por qué «Recopilado» y no «Compartido»:** el destino es **el propio Google Drive del usuario** (permiso `drive.file`); el desarrollador no recibe los datos ni los comparte con terceros. Confirmar esta redacción en la consola, porque Play es estricto con este punto.

## 3. Prácticas de seguridad (declarar)

- Cifrado en tránsito: **sí**.
- Base local cifrada en el dispositivo: **sí** (Keystore / DPAPI).
- Copia opcional en la nube cifrada con contraseña del usuario: **disponible**; **por defecto, sin contraseña** ⇒ declararlo con honestidad si Play pregunta por el cifrado en reposo.
- Excluida de las copias de seguridad de Android: **sí** (`allowBackup=false`).
- Sin analítica, publicidad ni telemetría: **sí**.

## 4. Otras secciones del formulario

- **Público objetivo:** adultos (docentes). **No** dirigida a menores de 13 años.
- **Contenido generado por usuarios:** no.
- **Anuncios:** no.
- **Compras dentro de la app:** no.
- **Permisos sensibles:** biometría (`USE_BIOMETRIC`), uso normal.
- **Eliminación de cuenta/datos:** no hay cuentas propias; el borrado es local + en el Drive del usuario. Añadir en la ficha de la tienda una URL con instrucciones de borrado.

## 5. Antes de enviar

1. Publicar `POLITICA_PRIVACIDAD.md` en una URL pública y ponerla en la ficha y en la app.
2. Poner las mismas respuestas del formulario en el aviso de privacidad para que no se contradigan.
3. Revisar si la cuenta de desarrollador exige prueba cerrada con testers antes de producción.
