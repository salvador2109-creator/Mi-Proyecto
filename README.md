
# 1. Crear la carpeta del proyecto
mkdir proyecto-calidad-software
cd proyecto-calidad-software

# 2. Inicializar el repositorio local
git init

# 3. Crear el archivo README.md
echo "# Proyecto Calidad" > README.md

# 4. Crear el commit inicial
git add .
git commit -m "feat: commit inicial - estructura base"

# 5. Conectar con el repositorio de GitHub
# Primero crea un repositorio VACÍO en GitHub
git remote add origin https://github.com/TU_USUARIO/proyecto-calidad-software.git

# 6. Establecer la rama principal y subirla
git branch -M main
git push -u origin main

# 7. Crear una rama para las figuras geométricas
git checkout -b feature/figuras-geometricas

# 8. Crear o modificar los archivos de código
# Ejemplo: main.py

# 9. Guardar los cambios
git add .
git commit -m "feat: añade calculo de areas refactorizado"

# 10. Subir la rama de funcionalidad
git push -u origin feature/figuras-geometricas

# 11. Regresar a la rama principal
git checkout main

# 12. Fusionar los cambios
git merge feature/figuras-geometricas

# 13. Subir los cambios fusionados
git push origin main
