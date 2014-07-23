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

Con el repositorio creado procedemos a inicializar el repositorio y asociarlo a github:

```sh
mkdir git4noobs
cd git4noobs
git init
git remote add origin https://github.com/{{usuario}}/git4noobs.git
```

##Paso 3

Usamos el comando log para ver los cambios en el repositorio:

```sh
git log
```

Para mas detalles con el comando git log se puede revisar la siguiente [documentación](http://git-scm.com/book/en/Git-Basics-Viewing-the-Commit-History).

##Paso 4

Creamos un archivo denominado main.js, para eso digitamos el siguiente comando:

```sh
vim main.js
```

Una vez dentro del archivo agregamos el siguiente contenido:

```js
(function(){
	
})();
```

Para ver el cambio que se efectuó en el repositorio creado ejecutamos el siguiente comando:

```sh
git status
```

El resultado debe ser este:

```sh
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	main.js

no changes added to commit (use "git add" and/or "git commit -a")
```

