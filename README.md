## Crear proyecto local en github

```bash
 git init 
```
genera la siguiente salida
```
ayuda: Usando 'master' como el nombre de la rama inicial. Este nombre de rama predeterminado
ayuda: está sujeto a cambios. Para configurar el nombre de la rama inicial para usar en todos
ayuda: de sus nuevos repositorios, reprimiendo esta advertencia, llama a:
ayuda: 
ayuda:  git config --global init.defaultBranch <nombre>
ayuda: 
ayuda: Los nombres comúnmente elegidos en lugar de 'master' son 'main', 'trunk' y
ayuda: 'development'. Se puede cambiar el nombre de la rama recién creada mediante este comando:
ayuda: 
ayuda:  git branch -m <nombre>
Inicializado repositorio Git vacío en /home/salas/Documentos/WEB/cv/.git/
```

## Revisar que ya se creó la carpeta .git

```bash
$ ls -la
```

salida 
```
total 24
drwxrwxr-x 5 salas salas 4096 sep 18 18:06 .
drwxr-xr-x 4 salas salas 4096 sep 14 18:03 ..
drwxrwxr-x 2 salas salas 4096 sep 14 18:05 css
drwxrwxr-x 7 salas salas 4096 sep 18 18:06 .git
drwxrwxr-x 2 salas salas 4096 sep 17 18:20 imgs
-rw-rw-r-- 1 salas salas 3656 sep 17 18:21 index.html
```


## Agregar un archivo al repositorio local

```bash
$ git add index.html 
```

## Agregar todos los archivos no actualizados al repositorio local

```bash
$ git add . 
```

## Crear un commit
```bash
$ git commit -m "inicial"
```

## Si no estas logueado entonces hay que configurar el usuario y correo para git

* Genera error si no está identificado en el sistema actual

```
Identidad del autor desconocido

*** Por favor cuéntame quién eres.

Ejecuta

  git config --global user.email "you@example.com"
  git config --global user.name "Tu Nombre"

para configurar la identidad por defecto de tu cuenta.
Omite --global para configurar tu identidad solo en este repositorio.

fatal: no es posible auto-detectar la dirección de correo (se obtuvo 'salas@salas.(none)')

```

Para mi caso:

```bash
$ git config --global user.email "micorreo@gs.utm.mx"
```

```bash
$  git config --global user.name  "Mi nombre"
```

## Generar el commit

```bash
$ git commit -m "inicial"
```

Se obtiene la salida

```bash
[master (commit-raíz) 87eefd5] inicial
 3 files changed, 327 insertions(+)
 create mode 100644 css/styles.css
 create mode 100644 imgs/bonita.png
 create mode 100644 index.html

 ```