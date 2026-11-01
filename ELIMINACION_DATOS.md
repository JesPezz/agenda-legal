# Instrucciones para la eliminación de datos — Agenda Escolar

**Última actualización:** 31 de octubre de 2026 · **Versión de la app:** 18.8 (escritorio) / 17.10.0, código 6180 (Android)

*Agenda Escolar* no tiene cuentas propias ni servidores del desarrollador: los datos están en tu equipo y, si lo activaste, en **tu** Google Drive. Por eso la eliminación la ejecutas tú, en cuatro pasos posibles (basta con los que te correspondan).

## 1. Borrar los datos desde la aplicación

**Android:** abre *Agenda Escolar* → **Alumnos** → icono de la **papelera** en la barra superior (**Borrar base de datos**) → **Borrar**. Se eliminan alumnos, asistencias, evaluaciones, tareas, calificaciones, expediente, diagnóstico, lectura, directorio y los datos de escuela y docente de **ese** teléfono.

**Windows:** *Agenda Escolar* → **Configuración** → grupo «Mantenimiento de la base de datos» → **Borrar base** → confirma.

El borrado también se propaga a la copia de Drive la próxima vez que sincronices, para que el curso no vuelva a aparecer.

## 2. Borrar los puntos de restauración

Las copias de seguridad se guardan **aparte** de la base y no siempre se borran con ella:

- **Windows:** abre la carpeta `C:\Users\<tu usuario>\AgendaEscolarData\respaldos\` y borra los archivos `respaldo_*.json` y `respaldo_*.json.cif`.
- **Android:** los puntos viven en el almacenamiento privado de la app; se eliminan al usar **Borrar datos** en los ajustes de Android o al desinstalar.

## 3. Borrar la copia en Google Drive

1. Entra en <https://drive.google.com> con la cuenta que usaste en la app.
2. Busca el archivo **`agenda_datos.json`** (el que crea la app al sincronizar).
3. Clic derecho → **Mover a la papelera** y luego **Vaciar papelera**.
4. Opcional pero recomendado: en <https://myaccount.google.com/permissions> retira el acceso de *Agenda Escolar*.

Google conserva además un historial de versiones del archivo durante unos 30 días; al vaciar la papelera deja de estar accesible desde la app.

## 4. Desinstalar la aplicación

- **Android:** mantén pulsado el icono → **Desinstalar** (o Ajustes → Aplicaciones → *Agenda Escolar* → Desinstalar). También puedes usar **Borrar datos** si solo quieres vaciarla sin quitarla.
- **Windows:** Configuración → Aplicaciones → *Agenda Escolar* → Desinstalar. Después, si quieres, borra la carpeta `AgendaEscolarData`.

## Borrado a distancia (varios equipos con la misma copia)

Si tienes la app en más de un equipo vinculado a la misma copia de Drive, puedes ordenar el borrado desde otro teléfono vinculado: el equipo afectado pierde sus datos locales, sus puntos de restauración y su vínculo con la cuenta la próxima vez que se conecte, sin necesidad de tenerlo en la mano. Si el aparato perdido nunca vuelve a abrir la app, no recibe la orden; en ese caso sus datos siguen cifrados y puedes revocar el acceso de Google y borrar la copia de Drive (paso 3).

## Contacto

Si algo de esto no funciona como se describe, escribe a **agendaescolarappzz@gmail.com** indicando el equipo y la versión de la app.
