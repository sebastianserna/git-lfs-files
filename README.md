# Git LFS Files

Prueba de repositorio con Git Large File Storage (LFS). Incluye ejemplos de archivos 3D, imágenes, audio, video y otros formatos.

### Utilizar Git LFS en tu repositorio

#### Paso 0 

Instalar Git LFS https://git-lfs.github.com/

#### Paso 1

Crear un nuevo repositoro en Github al que le activarás Git LFS.

#### Paso 2 

Clonar repositorio en equipo local

#### Paso 3

Abrir repositorio en terminal y ejecutar el siguiente comando:

```
git lfs install --local
```

#### Paso 4

Añadir los formatos de archivo a los que queremos hacerle tracking con LFS

```
git lfs track "*.png,*.jpg,*.jpeg,*.webp,*.tif,*.tiff,*.gif,*.bmp,*.xcf,*.psd,*.svg,*.ai,*.eps,*.pdf,*.cdr,*.sketch,*.fig,*.raw,*.dng,*.cr2,*.nef,*.avi,*.mov,*.mpeg,*.mpg,*.m2v,*.mp4,*.mkv,*.webm,*.wmv,*.ogv,*.wav,*.mp3,*.m4a,*.ogg,*.oga,*.aep,*.prproj,*.blend,*.obj,*.gltf,*.glb,*.mtl,*.3ds,*.max,*.stl,*.fbx,*.dae,*.iges,*.step"
```

#### Paso 5

Añadir archivo de atributos al tracking de git:

```
git add .gitattributes
```

#### Paso 6

Se hace commit del archivo .gitattributes

```
git commit -m "Git LFS - Se incluye archivo .gitattributes"
```

#### Paso 7

Se hace push al repositorio

```
git push
```

#### Paso 8

Ya puedes añadir los archivos de imágenes y multimedia. Tu repositorio ya tiene activado y configurado Git LFS y Github almacenará los archivos con los formatos especificados en .gitattributes en su servidor dedicado para Git LFS.

Las cuentas gratuitas de Github tienen:

- 1GB Storage
- 1GB Bandwidth (Bandwidth quota resets in 11 days)

Puedes verificar tu consumo en:
https://github.com/settings/billing

En caso de necesitar mayor storage Github ofrece un plan desde 5 USD al mes por 50GB de almacenamiento. 


### Referencias y tutoriales

- Git LFS website https://git-lfs.github.com/
- Git LFS repo https://github.com/git-lfs/git-lfs
- Configuring Git Large File Storage https://help.github.com/en/github/managing-large-files/configuring-git-large-file-storage
- Working with Blender, Git and Git Large File Storage (LFS) https://creativepolygon.com/tutorials/working-with-blender-git-and-git-large-file-storage-lfs


### Créditos de archivos de ejemplo

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
