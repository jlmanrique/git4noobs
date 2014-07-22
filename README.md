Git4Noobs
=========

##Paso 1

Crear el repositorio desde la linea de comandos:

```
curl -u '{{usuario}}' https://api.github.com/user/repos -d '{"name":"{{repositorio}}"}'
```

Donde:
 - usuario : usuario de github
 - repositorio : nombre del repositorio a crear

##Paso 2

Usamos el comando log para ver los cambios en el repositorio

```
git log
```
