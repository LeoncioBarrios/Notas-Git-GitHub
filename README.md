# Notas-Git-GitHub

## Comandos básicos de Git


### Configurar Git

**Establecer configuración global obligatoria**
git config --global user.name "nombre de usuario"
git config --global user.email "correo@electronico.com"

**Otros comandos de configuración**
git config --list    <= Lista todas la propiedades configuradas.
git config <clave>   <= Permite ver el valor de una clave en específico.

**Obtener ayuda**

git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/LeoncioBarrios/NSiaya.git
git push -u origin main
