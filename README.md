# Notas-Git-GitHub

## Comandos básicos de Git

<br>

### Configurar Git

**Establecer configuración global obligatoria**

git config --global user.name "nombre de usuario"<br>
git config --global user.email "correo@electronico.com"<br>


**Otros comandos de configuración**

git config --list    <= Lista todas la propiedades configuradas.<br>
git config \<clave>   <= Permite ver el valor de una clave en específico.<br>

<br>

**Obtener ayuda**

git help<br>
git help \<verbo><br>
git \<verbo> --help<br>

### Iniciar un repositorio local

git init <br>
git add \<archivo> |  \<patrón de archivos> | \< . > <br>
git commit -m "comentario alusivo al commit" <br>

<br>

### Subir un repositorio local a un repositorio remoto

git init <br>
git add \<archivo> |  \<patrón de archivos> | \< . > <br>
git commit -m "comentario alusivo al commit" <br>
git remote add origin \<url repositorio remoto> <br>
git push -u origin \<branch> <br>


### Trabajar con ramas.

**Crear una nueva rama** <br>
  git branch _nombre_nueva_rama_

**Cambiar de rama** <br>
  git checkout _nombre_rama_

**Crear y cambiarse a la nueva rama** <br>
  git checkout -b _nombre_nueva_rama_

**Renombrar una rama** <br>
  git branch -m _viejo_nombre_rama_ _nuevo_nombre_rama_ <br>
  
  ó <br>
  
  git branch --move _viejo_nombre_rama_ _nuevo_nombre_rama_ <br>

