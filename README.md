# Curso Git desde cero

## ¿Qué es Git?

Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos.


## Zonas de Git

1. Directorio de trabajo
2. Área de preparación
3. Directorio Git


## Configurar Git por primera vez

```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git config --global core.editor code
git config --list
```

## Configuración SSH en Windows

Usando Git Bash seguimos los siguientes pasos:

0. Es buena práctica tener una carpeta en el raíz de `C` para evitar problemas de rutas.

1. Ejecutamos el comando ssh-keygen -t rsa -b 4096 -C correo@ejemplo.com
Es conveniente usar el mismo correo con el que nos registramos en GitHub. Indicamos la ruta y un nombre pa identificarla.

2. Iniciamos ss-agente en background ejecutando el comando `eval "$(ss-agent -s)"`.

3. Agragamos la llave ssh generada a ssh-agente ejecutando el comando `ssh-add RUTA`. Ejemplo de ruta `/c/llaves-ssh/github_rsa`.

4. Usamos el comando `cat`para ver nuestra llave pública y añadirla a Github. Ejemplo, `cat /c/llaves-ssh-github_rsa.pub`.
Con este comando vemos el contenido del archivo, tenemos que copiar todo el texto mostrado.

5. Vamos a configuración de nuestro perfil de Github y añadimos la llave SSH copiada.

A partir de ahora ya podemos hacer pull y push sin que Github nos pida los datos de acceso cada vez.


## Flujo de trabajo básico en Git

1. Modificas una serie de archivos en tu directorio de trabajo.
2. Preparar los archivos anadiéndolos al área de preparación.
3. Confirmar los cambios, tomando los archivos tal y como están en el área de preparación y almacenar esa copia instantánea de manera permanente en tu directorio de Git.
