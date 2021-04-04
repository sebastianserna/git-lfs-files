# Git LFS Files

Prueba de repositorio con Git Large File Storage (LFS). Incluye ejemplos de archivos 3D, imágenes, audio, video y otros formatos.

## Utilizar Git LFS en tu repositorio

### Paso 0 

Instalar Git LFS https://git-lfs.github.com/

### Paso 1

Crear un nuevo repositoro en Github al que le activarás Git LFS.

### Paso 2 

Clonar repositorio en equipo local

### Paso 3

Abrir repositorio en terminal y ejecutar el siguiente comando:

```
git lfs install
```

Si prefieres instalarlo en local puedes utilizar el flag `--local`

```
git lfs install --local
```

### Paso 4

Añadir los formatos de archivo a los que queremos hacerle tracking con LFS.

Puedes utilizar el comando `git lfs track` especificando la extensión del archivo:

```
git lfs track *.jpg
```

La primera vez que utilices el comando se creará un archivo `.gitattributes` incluyendo el formato especificado, puedes utilizar el comando cuantas veces quieras para añadir nuevos formatos al archivo.

También puedes crear el archivo `.gitattributes` manualmente y le incluyes los formatos a los que deseas hacer tracking, a continuación encuentras un listado de formatos comunes de archivos de audio, video, imagen, 3D y otros, puedes copiar el siguiente bloque de texto en tu archivo `.gitattributes`:

```
*.xcf filter=lfs diff=lfs merge=lfs -text
*.ogv filter=lfs diff=lfs merge=lfs -text
*.mp3 filter=lfs diff=lfs merge=lfs -text
*.ogg filter=lfs diff=lfs merge=lfs -text
*.blend filter=lfs diff=lfs merge=lfs -text
*.stl filter=lfs diff=lfs merge=lfs -text
*.webp filter=lfs diff=lfs merge=lfs -text
*.gif filter=lfs diff=lfs merge=lfs -text
*.psd filter=lfs diff=lfs merge=lfs -text
*.cdr filter=lfs diff=lfs merge=lfs -text
*.raw filter=lfs diff=lfs merge=lfs -text
*.m2v filter=lfs diff=lfs merge=lfs -text
*.oga filter=lfs diff=lfs merge=lfs -text
*.dae filter=lfs diff=lfs merge=lfs -text
*.jpeg filter=lfs diff=lfs merge=lfs -text
*.svg filter=lfs diff=lfs merge=lfs -text
*.pdf filter=lfs diff=lfs merge=lfs -text
*.fig filter=lfs diff=lfs merge=lfs -text
*.mov filter=lfs diff=lfs merge=lfs -text
*.png filter=lfs diff=lfs merge=lfs -text
*.tif filter=lfs diff=lfs merge=lfs -text
*.nef filter=lfs diff=lfs merge=lfs -text
*.glb filter=lfs diff=lfs merge=lfs -text
*.3ds filter=lfs diff=lfs merge=lfs -text
*.tiff filter=lfs diff=lfs merge=lfs -text
*.cr2 filter=lfs diff=lfs merge=lfs -text
*.mpeg filter=lfs diff=lfs merge=lfs -text
*.webm filter=lfs diff=lfs merge=lfs -text
*.wmv filter=lfs diff=lfs merge=lfs -text
*.bmp filter=lfs diff=lfs merge=lfs -text
*.ai filter=lfs diff=lfs merge=lfs -text
*.sketch filter=lfs diff=lfs merge=lfs -text
*.wav filter=lfs diff=lfs merge=lfs -text
*.prproj filter=lfs diff=lfs merge=lfs -text
*.obj filter=lfs diff=lfs merge=lfs -text
*.step filter=lfs diff=lfs merge=lfs -text
*.jpg filter=lfs diff=lfs merge=lfs -text
*.eps filter=lfs diff=lfs merge=lfs -text
*.avi filter=lfs diff=lfs merge=lfs -text
*.mkv filter=lfs diff=lfs merge=lfs -text
*.aep filter=lfs diff=lfs merge=lfs -text
*.gltf filter=lfs diff=lfs merge=lfs -text
*.max filter=lfs diff=lfs merge=lfs -text
*.fbx filter=lfs diff=lfs merge=lfs -text
*.iges filter=lfs diff=lfs merge=lfs -text
*.dng filter=lfs diff=lfs merge=lfs -text
*.mpg filter=lfs diff=lfs merge=lfs -text
*.mp4 filter=lfs diff=lfs merge=lfs -text
*.m4a filter=lfs diff=lfs merge=lfs -text
*.mtl filter=lfs diff=lfs merge=lfs -text
*.zip filter=lfs diff=lfs merge=lfs -text
*.bin filter=lfs diff=lfs merge=lfs -text
*.arproj filter=lfs diff=lfs merge=lfs -text
*.lsproj filter=lfs diff=lfs merge=lfs -text
```

También puedes utilizar una lista más reducida de formatos solo de imagen, video y 3D

```
*.jpeg filter=lfs diff=lfs merge=lfs -text
*.jpg filter=lfs diff=lfs merge=lfs -text
*.png filter=lfs diff=lfs merge=lfs -text
*.svg filter=lfs diff=lfs merge=lfs -text
*.webp filter=lfs diff=lfs merge=lfs -text
*.gif filter=lfs diff=lfs merge=lfs -text
*.psd filter=lfs diff=lfs merge=lfs -text
*.ai filter=lfs diff=lfs merge=lfs -text
*.fig filter=lfs diff=lfs merge=lfs -text
*.sketch filter=lfs diff=lfs merge=lfs -text
*.avif filter=lfs diff=lfs merge=lfs -text
*.eps filter=lfs diff=lfs merge=lfs -text
*.pdf filter=lfs diff=lfs merge=lfs -text
*.tiff filter=lfs diff=lfs merge=lfs -text
*.tif filter=lfs diff=lfs merge=lfs -text
*.raw filter=lfs diff=lfs merge=lfs -text
*.cr2 filter=lfs diff=lfs merge=lfs -text
*.nef filter=lfs diff=lfs merge=lfs -text
*.arw filter=lfs diff=lfs merge=lfs -text
*.dng filter=lfs diff=lfs merge=lfs -text
*.cdr filter=lfs diff=lfs merge=lfs -text
*.m2v filter=lfs diff=lfs merge=lfs -text
*.mov filter=lfs diff=lfs merge=lfs -text
*.mpeg filter=lfs diff=lfs merge=lfs -text
*.webm filter=lfs diff=lfs merge=lfs -text
*.wmv filter=lfs diff=lfs merge=lfs -text
*.mpg filter=lfs diff=lfs merge=lfs -text
*.mp4 filter=lfs diff=lfs merge=lfs -text
*.m4a filter=lfs diff=lfs merge=lfs -text
*.bmp filter=lfs diff=lfs merge=lfs -text
*.wav filter=lfs diff=lfs merge=lfs -text
*.prproj filter=lfs diff=lfs merge=lfs -text
*.obj filter=lfs diff=lfs merge=lfs -text
*.step filter=lfs diff=lfs merge=lfs -text
*.avi filter=lfs diff=lfs merge=lfs -text
*.mkv filter=lfs diff=lfs merge=lfs -text
*.aep filter=lfs diff=lfs merge=lfs -text
*.blend filter=lfs diff=lfs merge=lfs -text
*.3ds filter=lfs diff=lfs merge=lfs -text
*.gltf filter=lfs diff=lfs merge=lfs -text
*.glb filter=lfs diff=lfs merge=lfs -text
*.max filter=lfs diff=lfs merge=lfs -text
*.fbx filter=lfs diff=lfs merge=lfs -text
*.mtl filter=lfs diff=lfs merge=lfs -text
*.zip filter=lfs diff=lfs merge=lfs -text
*.rar filter=lfs diff=lfs merge=lfs -text
*.bin filter=lfs diff=lfs merge=lfs -text
*.arproj filter=lfs diff=lfs merge=lfs -text
*.lsproj filter=lfs diff=lfs merge=lfs -text
```

### Paso 5

Añadir archivo de atributos al tracking de git:

```
git add .gitattributes
```

### Paso 6

Se hace commit del archivo `.gitattributes`

```
git commit -m "Git LFS - Se incluye archivo .gitattributes"
```

### Paso 7

Se hace push al repositorio

```
git push
```

### Paso 8

Puedes añadir los archivos de imágenes y multimedia. Tu repositorio ya tiene activado y configurado Git LFS y Github almacenará los archivos con los formatos especificados en `.gitattributes` en su servidor dedicado para Git LFS.

Las cuentas gratuitas de Github tienen:

- 1GB Storage
- 1GB Bandwidth (hace reset cada mes)

Puedes verificar tu consumo en:
https://github.com/settings/billing

En caso de necesitar mayor storage Github ofrece un plan desde 5 USD al mes por 50GB de almacenamiento. 

---

## Referencias y tutoriales

- Git LFS website https://git-lfs.github.com/
- Git LFS repo https://github.com/git-lfs/git-lfs
- Configuring Git Large File Storage https://help.github.com/en/github/managing-large-files/configuring-git-large-file-storage
- Working with Blender, Git and Git Large File Storage (LFS) https://creativepolygon.com/tutorials/working-with-blender-git-and-git-large-file-storage-lfs


## Créditos de archivos de ejemplo

Swanix 
https://swanix.org

File Examples 
https://file-examples.com/

Freepik
https://www.freepik.es/

Google Developers
https://developers.google.com/speed/webp/gallery1

Gimp
https://www.gimp.org/tutorials/Floating_Logo/

Mixkit
https://mixkit.co/free-premiere-pro-templates/

Google Poly
https://poly.google.com/view/5XpesCyaPe-

CGTrader
https://www.cgtrader.com/free-3d-models/architectural/decoration/bunny-toy
