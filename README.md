# Notas-Git-GitHub

## Comandos básicos de Git

<br>

### Configurar Git

**Establecer configuración global obligatoria**

```
git config --global user.name "nombre de usuario"
git config --global user.email "correo@electronico.com"
```

**Otros comandos de configuración**
```
git config --list    <= Lista todas la propiedades configuradas.
git config \<clave>   <= Permite ver el valor de una clave en específico.
```
<br>

**Obtener ayuda**
```
git help
git help \<verbo>
git \<verbo> --help
```
### Iniciar un repositorio local
```
git init
git add \<archivo> |  \<patrón de archivos> | \< . >
git commit -m "comentario alusivo al commit"
```

<br>

### Subir un repositorio local a un repositorio remoto
```
git init
git add \<archivo> |  \<patrón de archivos> | \< . >
git commit -m "comentario alusivo al commit"
git remote add origin \<url repositorio remoto>
git push -u origin \<branch>
```

### Trabajar con ramas.

**Crear una nueva rama**
```
git branch nombre_nueva_rama
```

**Cambiar de rama**
```
git checkout nombre_rama
```
**Crear y cambiarse a la nueva rama**
```
git checkout -b nombre_nueva_rama
```

**Renombrar una rama**
```
git branch -m viejo_nombre_rama nuevo_nombre_rama

ó

git branch --move viejo_nombre_rama nuevo_nombre_rama
```

**Eliminar una rama**  <br>
No se puede eliminar la rama actual, primero hay que moverse a otra rama, de ser el caso.

```
git branch -d nombre_rama_a_eliminar

ó

git branch --delete nombre_rama_a_eliminar
```

Forzar la eliminación si existen cambios no actualizados en la rama a eliminar:

```
git branch -D nombre_rama_a_eliminar

ó

git branch -d --force nombre_rama_a_eliminar

ó

git branch --delete --force nombre_rama_a_eliminar
```
**Fusionar ramas**

* Primero debemos ubicarnos en la rama que va a recibir la fusión.
* Luego ejecutar el comando:

```
git merge rama_a_fusionar
```

El procedimiento sería:

```
git checkout master
git merge rama_a_fusionar
git branch -d rama_a_fusionar
```
