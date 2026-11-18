[Versión 0.7.2]: #
# downyt - Descargador de vídeos de youtube, wrapper de yt-dlp

Se trata de un wrapper de [yt-dlp](https://github.com/yt-dlp), se puede usar de forma independiente pero se desarrolló como herramienta para [Meritxell](https://github.com/4lexKy/meritxell). Se actualiza automáticamente y descarga 4 versiones (audio-Mejor, 1080p-AV1, 1080p-MaxBitRate, resolución máxima).

---
## Estado del proyecto
Actualmente funciona correctamente.

### Ficheros
- downyt: fichero principal del proyecto
- LICENSE: contenido de la licencia
- README.md: información del proyecto
- .gitignore: define elementos a ignorar

---
## Instalación
No requiere instalación
- [yt-dlp](https://github.com/yt-dlp) (descarga automática, no requiere instalación manual)

### Lenguaje
- Bash

### Dependencias
Sí, tiene dependencias de:
- ffmpeg (Debian/Ubuntu)
- python3 (Debian/Ubuntu)
- nodejs (Debian/Ubuntu)
- curl (Debian/Ubuntu)

### Sistemas operativos compatibles
Probado en:
- Debian

---
## Uso
No se requiere instalación. Para usar símplemente se ha de ejecutar el script principal. A continuación se pueden ver las diferentes opciones de ejecución y descarga

### Opciones de ejecución: EXCLUYENTES (solo 1 opción a la vez)
- **-h** -> Muestra la información de uso del programa por terminal
- **-i URLyoutube** -> Muestra la información de descarga del vídeo (sin descarga)
- **-a URLyoutube** -> Descarga solo el audio del vídeo
- **-v X URLyoutube** -> Descarga el vídeo (con audio) según la opción 'X' indicada. Las opciones pueden ser:

>>**a** o **A** -> Descarga el vídeo en 1080p con códec AV1

>>**b** o **B** -> Descarga el vídeo en 1080p con el máximo bitrate

>>**c** o **B** -> Descarga el vídeo en la máxima resolución existente
- **-t URLyoutube** -> Descarga las 4 versiones a la vez (audio + 1080-AV1 + 1080-MaxBR + MaxRes)

### Opciones de ejecución: Se pueden combinar entre sí y con las anteriores
- **-n URLyoutube** -> La salida estándar del programa es el nombre que quedará tras las descarga. Útil para gestión de las descargas
- **-l** -> Si es una lista de reproduccion la descarga. Solo tiene efecto junto a las opciones de descarga
- **-p rutaDeDescarga** -> Solo tiene efecto junto a las opciones de descarga.

*De forma predeterminada NO se descargan las listas de reproducción.

---
## Recomendación
Para un uso mas ágil se puede crear una carpeta para script de forma que todos los que se añadan se puedan llamar desde la propia terminal como cualquier otro comando.

Esto se puede conseguir añadiendo a ~/.bashrc la línea:

```bash
    export PATH=$PATH:/ruta/a/carpeta/con/scripts
```

---
## Licencia
Este proyecto está licenciado bajo GPLv2 - consulta el archivo LICENSE para más detalles.

---
## Autor
>**Alex**
- Github: [https://github.com/4lexKy](https://github.com/4lexKy)
- Email: [alex.correu@pm.me](mailto:alex.correu@pm.me)

---
