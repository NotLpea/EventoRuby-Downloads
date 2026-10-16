# Evento Ruby · Distribución de Pruebas

Manifiestos de actualización y mods propios autorizados para Evento Ruby Launcher. Minecraft 1.21.1, Fabric Loader 0.19.5 y Java 21; 43 mods sin AnimatedFrames ni WaterMedia.

Cada Release publicada incluye `pruebas.lock.json`, los dos JAR propios y `SHA256SUMS.txt`. Los demás mods se descargan de sus fuentes oficiales. El launcher verifica los hashes y abre la instancia exclusiva mediante Prism.

Para actualizar el modpack, preparar una rama y un Pull Request con el nuevo inventario en `release-inputs/pruebas.lock.json`. Fijar versiones, dependencias, tamaños, hashes y URLs oficiales de los archivos de terceros. Colocar únicamente binarios propios con permiso en `release-inputs/`, y actualizar `release.json` con una revisión y etiqueta nuevas. No sobrescribir una versión publicada.

La primera publicación se prepara desde la rama `release/pruebas-1.0.0`. El tag identifica los archivos de entrada auditados. La automatización añade las URLs que devuelve GitHub tras subir los assets y publica el manifiesto solo cuando están completos. Una Release marcada como latest pasa a ser la distribución que reciben los launchers; las siguientes publicaciones requieren revisión y pruebas antes de ejecutarse.

Consultar `PERMISOS.md`. Los JAR de terceros y los datos privados de Prism quedan fuera de esta distribución.
