

- **Alumno:** islem benbeztout
- **Bloque:** B0 — Prerrequisitos
- **Fase / ejercicio:** Fase 0.8
- **Fecha de inicio:** 22/10/2026
- **Fecha de entrega:** 22/00/2026

---

## 🎯 Qué se pedía

Crear desde cero una bóveda en Obsidian  con su estructura de carpetas, un proyecto web de préstamo de portátiles y un repositorio Git conectado por SSH. Había que guardar tres versiones además de grabar todo el proceso en pantalla con marcas de tiempo y completar la bitácora.

## ⌨️ Comandos y pasos importantes

- `comando` —
- `git --version`, `git config`, `ssh -T git@github.com` — para comprobar la disponibilidad de Git, la identidad del autor y la autenticación SSH.

- `pwd` — para verificar que nos encontramos en la ruta exacta del proyecto (`01_Proyecto`) antes de inicializar Git.
    
- `git init` y `git branch -M main` — para inicializar el repositorio local y establecer la rama principal como `main`.
    
- `git remote add origin <url>` y `git remote -v` — para registrar y verificar la dirección remota de GitHub.
    
- `git status` — para comprobar el estado de los archivos (sin seguimiento, modificados o preparados).
    

    
- `git add <ruta>` — para preparar los cambios específicos que formarán parte del siguiente commit.

- `git diff` y `git diff --cached` — para comparar los cambios realizados en los archivos respecto al índice o al último commit.
    


- `git commit -m "mensaje"` — para guardar localmente una versión con los cambios preparados y una descripción.
    
    

- `git push` — para subir los commits locales al repositorio remoto en GitHub.

    

- `git check-ignore -v` — para comprobar qué regla del `.gitignore` está excluyendo los archivos de vídeo.
    
- `git log --oneline` — para consultar el historial de versiones con códigos abreviados.
    
- `git switch --detach <codigo>` y `git switch main` — para viajar temporalmente a un commit anterior y regresar a la rama principal..

## 🛠️ Qué he hecho

- Primero comprobé que las herramientas funcionaban bien, creé la carpeta del proyecto con su estructura, configuré los bloqueos para los vídeos y dejé lista la primera página web.

- Después activé el control de versiones, lo conecté con el repositorio en internet y guardé la primera versión y la segunda modificación del estado del equipo.

- Más adelante añadí las páginas nuevas, una imagen y los enlaces correspondientes, revisando que todo estuviera en orden para guardar la tercera versión.

- Por último, comprobé el historial para ver que podía moverme entre la versión antigua y la actual sin problemas, grabé la pantalla, añadí el enlace del vídeo en la bitácora y subí el cierre final.
## 🚩 Qué me ha fallado y cómo lo he resuelto
En un apartado no se copiaban los comandos hasta que descargué el PDF con la ayuda de Pedro. Además, en otro caso no me funcionaba el `cd` y tuve que revisar la extensión porque había un doble ".md"

## 🤔 Respuestas a las preguntas

## 1. ¿Por qué `git init` se hizo en `01_Proyecto` y no en la raíz de la bóveda?

Porque quería que Git controlara únicamente los archivos del proyecto web, sin incluir otros archivos o carpetas de la bóveda. Así, el historial del repositorio queda organizado y limitado al proyecto.

## 2. ¿Qué mostró `git status` antes de `add`, después de `add` y después de `commit`?

- Antes de `git add`: los archivos aparecían como no rastreados (untracked).
    
- Después de `git add`: los archivos aparecían preparados para el próximo commit (staged).
    
- Después de `git commit`: los cambios quedaron guardados en el historial y el directorio de trabajo quedó limpio, si no había otros cambios pendientes.
    

## 3. ¿Por qué creaste un repositorio de GitHub propio y lo conectaste con `git remote add origin`?

Creé un repositorio propio en GitHub para tener una copia remota del proyecto y poder compartirlo o recuperarlo si fuera necesario. Utilicé `git remote add origin` para conectar mi repositorio local con el repositorio remoto de GitHub.

## 4. ¿Por qué las páginas nuevas aparecen en `git status` pero no en `git diff -- web/index.html`?

Porque `git status` muestra los archivos nuevos que Git todavía no está rastreando, mientras que `git diff -- web/index.html` muestra los cambios en archivos que Git ya conoce, comparándolos con el directorio de trabajo. Para ver los archivos nuevos, primero hay que añadirlos con `git add` o consultar su contenido directamente.

## 5. ¿Cómo has comprobado que los vídeos existen pero no se van a subir?

Comprobé que los vídeos estaban en la carpeta del proyecto y revisé el archivo `.gitignore` para verificar que sus rutas o extensiones estuvieran excluidas. También podía comprobarlo con `git status --ignored` y confirmar que no aparecían entre los archivos preparados para subir.

## 6. ¿Qué muestra `git diff --cached --stat` después de preparar los cuatro archivos?

Muestra un resumen de los cambios preparados para el próximo commit: los nombres de los archivos modificados, las líneas añadidas y eliminadas y el número de archivos afectados. En este caso, debería mostrar los cuatro archivos preparados, siempre que los cuatro estén incluidos en el área de preparación.

## 7. ¿Qué cambia al visitar el primer commit y qué recuperas al volver a `main`?

Al visitar el primer commit, puedo ver el estado que tenía el proyecto en ese momento, antes de los cambios posteriores. Al volver a `main`, recupero la versión correspondiente al estado actual de esa rama.

## 8. ¿Por qué esta web necesita historial? ¿Qué aportaría GitHub si otro técnico trabajase contigo?

El historial permite saber qué cambios se han realizado, cuándo se hicieron y recuperar versiones anteriores si aparece algún error. Si otro técnico trabajase conmigo, GitHub facilitaría compartir el código, revisar cambios, colaborar en distintas tareas y mantener una copia remota del proyecto.

## 9. Si mañana corriges una errata en `normas.html`, ¿qué pasos repites y cuáles no?

Repetiría los pasos necesarios para guardar el nuevo cambio:

1. Editar `normas.html` y corregir la errata.
    
2. Ejecutar `git status` para comprobar el cambio.
    
3. Ejecutar `git diff` para revisar la modificación.
    
4. Ejecutar `git add web/normas.html` para preparar el archivo.
    
5. Ejecutar `git diff --cached` para revisar el cambio preparado.
    
6. Ejecutar `git commit -m "Corrige errata en normas.html"` para guardarlo en el historial.
    
7. Ejecutar `git push` para enviar el nuevo commit a GitHub, si el repositorio remoto ya está configurado.

## 🔗 Enlaces

- **Vídeo de esta fase:**  https://youtu.be/BQ9FGuoQrPs?si=AQHeqHx5zR0SvVCv
- **Playlist:** https://www.youtube.com/playlist?list=PLQ0xCUR65674

## 💭 Dudas / a repasar

La verdad es que nada, todo está bien explicado. Las únicas dudas que me surgieron las resolví en clase.