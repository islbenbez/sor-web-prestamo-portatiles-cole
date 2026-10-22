

- **Alumno:** islem benbeztout
- **Bloque:** B0 — Prerrequisitos
- **Fase / ejercicio:** Fase 0.8
- **Fecha de inicio:** 22/10/2026
- **Fecha de entrega:** 22/00/2026

---

## 🎯 Qué se pedía

hacer una pagina web simple y subirla a github tambien crear repositorios y hacer push

## ⌨️ Comandos y pasos importantes

- `comando` — pwd git remote -v git status Qué significa cada línea: Línea Significado 1 Muestra la carpeta actual. 2 Muestra las direcciones de origin. 3 Identifica los cambios pendientes; debe aparecer la bitácora modificada.

## 🛠️ Qué he hecho

(Los pasos que has seguido. No copies el enunciado: cuenta lo que hiciste tú.)

## 🚩 Qué me ha fallado y cómo lo he resuelto

(El mensaje de error LITERAL y qué hiciste. Si no falló nada, escribe "nada"
— pero piénsalo dos veces antes.)

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
- **Playlist:** 

## 💭 Dudas / a repasar

- (lo que no te ha quedado claro)