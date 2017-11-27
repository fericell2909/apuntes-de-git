
# Zonas de Git
1. Directorio de Trabajo.
2. Pzona de Preparacion.
3. directorio Git.


## Flujo de trabajo basico en Git
1. Modificas una serie de archivos en tu directorio de trabajo.
2. Preparas los archivo, añadiendolos a tu area de preparacion.
3. Confirmas los cambios, lo que toma los archivos tal y como estan en el area de preparacion  y almacena esa copia instantanea de manera permanente en tu directorio Git.

## Configurando git por primera vez
```
git config --global user.name "Marco Estrada Lopez"
git config --global user.email "fericell2909@gmail.com"
git config --global core.editor subl
```

## Configuracion SSH en Windows
Usando Git Bash seguimos los siguientes pasos:
1. Creamos una carpeta llamada `llabes-ssh`

2.Ejecutamos el comando `ssh-keygen -t rsa -C "ejemplo@ejemplo.com"`
El correo debe se el mismo con el que nos registramos en GitHub para evitar posibles problemas.
Dejamos el passphrase vacio y damos enter.
Cuando nos pida la ruta escribimos `/c/llaves-ssh/github_rsa`

3.Iniciamos ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"

4.Agregamos la llave ssh generada a ssh-agent ejecutando el comando `ssh--add /c/llaves-ssh/github_rsa`.

5. Usar el comando `cat /c/llaves-ssh/github_rsa.pub`
Con este comando vemos el contenido del archivo, copiamos todo el texto que nos muestra.

6. Ir a las configuraciones de nuestro perfil de GitHub y agregar una nueva llave SSH con el contenido que hemos copiado de `github_rsa.pub`.

Desde ahora podemos hacer pull y push sin que Github no este pidiendo los datos de acceso.
