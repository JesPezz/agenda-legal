# Política de privacidad — Agenda Escolar

**Última actualización:** 31 de octubre de 2026

*Agenda Escolar* es una aplicación de escritorio (Windows) y para Android que permite al docente llevar la asistencia, las evaluaciones y los reportes de su grupo, y generar la agenda escolar en Word o PDF.

> Se publica en https://jespezz.github.io/agenda-legal/ y se enlaza desde la ficha de la tienda.

## Resumen

- **El desarrollador no recopila tus datos.** No hay servidores del desarrollador, ni cuentas propias, ni analítica, ni publicidad.
  En la ficha de Google Play, el envío opcional a **tu** Drive se declara como «recopilado» solo porque el dato sale del dispositivo; nunca llega a nosotros ni se comparte con terceros.
- **Tú decides dónde se guarda.** Todo vive en tu equipo (**arquitectura local-first**, sin servidores del desarrollador); opcionalmente puedes hacer copia en **tu** Google Drive.
- **Puedes borrarlo todo** desde la app, en cualquier momento. El paso a paso está en las [instrucciones para la eliminación de datos](https://jespezz.github.io/agenda-legal/eliminacion.html).

## Qué datos trata la app

Los que tú capturas o importas: datos de identificación del alumnado (nombre, CURP, fecha de nacimiento, edad, sexo, número de lista y matrícula), información escolar (asistencia, calificaciones, tareas, evaluaciones, lectura, expediente), datos de contacto de tutores y datos de la escuela y del docente.

## Finalidad

Prestar el servicio de la aplicación: registrar, calcular, resguardar y exportar la información escolar. Nada más.

## Almacenamiento y cifrado

| Dónde | Qué | Protección |
|---|---|---|
| Tu equipo | Base local | Cifrada en Android (Keystore); en Windows, protegida por la sesión del usuario |
| Puntos de restauración | Copias de la base | Cifrados (Keystore / DPAPI) |
| Tu Google Drive (opcional) | Copia sincronizada | Cifrado opcional con contraseña que tú eliges (por defecto va sin contraseña) |
| Comunicaciones | Sincronización | TLS |

La app **no se incluye** en las copias de seguridad automáticas de Android.

## Con quién se comparte

Con nadie, salvo Google, y solo si tú conectas tu cuenta de Drive: el archivo se guarda en **tu** unidad con el permiso `drive.file`. No tenemos acceso a él.

La aplicación es de **almacenamiento local desacoplado** (*local-first*): no hay flujo de datos hacia el desarrollador, que por ello **no actúa como encargado** del tratamiento ni necesita contrato de encargo contigo.

## Tus derechos y control

- **Acceso y exportación:** los reportes en Word/PDF los generas tú.
- **Supresión:** «Borrar base» elimina los datos del equipo; en Drive puedes borrar el archivo desde tu cuenta.
- **Derechos ARCO:** al no recopilar el desarrollador ningún dato, no puede tramitarlos; las solicitudes se dirigen al docente o a la institución educativa.
- **Borrado a distancia:** si vinculas varios teléfonos a la misma copia de Drive, puedes ordenar el borrado del teléfono anterior desde otro teléfono vinculado; el aparato afectado pierde sus datos locales y su vínculo con la cuenta **la próxima vez que se conecte** (si nunca vuelve a abrir la app, sus datos siguen cifrados en él).
- **Portabilidad:** la app no envía tus datos fuera de tu control.

## Datos de menores

La app es una herramienta para adultos (docentes). El tratamiento de los datos de los alumnos corresponde a la escuela y al docente, conforme a la normativa aplicable.

## Contacto

**agendaescolarappzz@gmail.com** · Desarrollador: **JesPezz**

## Cambios

Publicaremos cualquier cambio en esta misma página y en la ficha de la tienda, junto con la versión correspondiente.
