Git4Noobs
=========

##Paso 1

Crear el repositorio desde la linea de comandos:

```sh
curl -u '{{usuario}}' https://api.github.com/user/repos -d '{"name":"{{repositorio}}"}'
```
Este comando requerirá ingresar la contraseña del usuario ingresado.

Donde:
 - usuario : usuario de github
 - repositorio : nombre del repositorio a crear para este ejemplo se llamara git4noobs

##Paso 2

Con el repositorio creado procedemos a inicializar el repositorio y asociarlo a github

```sh
mkdir git4noobs
cd git4noobs
git init
git remote add origin https://github.com/{{usuario}}/git4noobs.git
```

##Paso 3

Usamos el comando log para ver los cambios en el repositorio

```sh
git log
```
