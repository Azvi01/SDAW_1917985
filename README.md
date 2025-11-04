# Repositorio SDAW_1917985

**Alumno:** Javier Díaz López  
**Asignatura:** Uso de repositorios digitales (Git)  
**Repositorio base para la práctica entregable.**

---
## Información técnica añadida desde rama 2
(COPIAR AQUÍ LA RESPUESTA POR EL COMANDO INDICADO EN EL
PÁRRAFO ANTERIOR)


## Descripción
Proyecto mínimo que contiene una página `index.html` con un botón que muestra el mensaje de bienvenida:

- `index.html` - página principal con botón.
- `script.js` - lógica para mostrar el mensaje "Hola Javier Díaz López ".
- `server.js` - servidor Node.js con Express para lanzar el proyecto localmente.
- `package.json` - dependencias y script de arranque.
- `.gitignore` - archivos a ignorar.

---

## Cómo levantar el servidor (paso a paso)

1. Clona el repositorio o sitúate en la carpeta del proyecto:
   ```bash
   git clone <URL-del-repositorio>
   cd SDAW_1917985
   ```
2. Instala dependencias:
   ```bash
   npm install
   ```
3. Ejecuta el servidor:
   ```bash
   npm start
   ```
   Luego abre `http://localhost:3000` en el navegador y pulsa el botón para ver el saludo.

---

## Flujo de trabajo Git recomendado (ejemplos de comandos)

### Inicializar y primer commit
```bash
git init
git config user.name "Tu Nombre"
git config user.email "tu.email@ejemplo.com"
git add .
git commit -m "init: proyecto base SDAW_1917985"
```

### Conectar al remoto (tras crear el repo en GitHub llamado SDAW_1917985)
```bash
git remote add origin https://github.com/tuUsuario/SDAW_1917985.git
git branch -M main
git push -u origin main
```

### Crear ramas (sustituye con los identificadores que te dé el profesor)
```bash
git checkout -b rama1_[NombreApellido]
# editar README.md añadiendo explicación de comandos
git add README.md
git commit -m "feat: añadir explicación de comandos en rama1"
git push -u origin rama1_[NombreApellido]

git checkout main
git checkout -b rama2_[NombreApellido]
# generar log de git en una línea y pegarlo en README.md (rama2)
git log --oneline > gitlog_one_line.txt
# o pegar una línea representativa en README.md
git add gitlog_one_line.txt README.md
git commit -m "feat: añadir git log --oneline en rama2"
git push -u origin rama2_[NombreApellido]
```

### Pull requests y merges
- En GitHub: crea Pull Request desde `rama1_[NombreApellido]` a `main` y otro desde `rama2_[NombreApellido]` a `main`.
- Resuelve conflictos si los hay desde la interfaz de GitHub o localmente (git merge, git restore, etc).
- No elimines las ramas; deben permanecer para evidenciar el trabajo.

---

## Contenido que debe añadirse en cada rama (según la práctica)

### Contenido sugerido para `rama1_[NombreApellido]` (explicación de comandos)
Añade en `README.md` una sección como:

```
## Información técnica añadida desde rama 1
- git init: Inicializa un repositorio local en la carpeta del proyecto.
- git add: Añade archivos al área de staging para preparar el commit.
- git commit: Crea un commit con los cambios añadidos al staging area.
- git branch: Lista, crea o elimina ramas.
- git merge: Fusiona cambios de una rama a otra.
- git push: Envía commits locales al repositorio remoto.
```

### Contenido sugerido para `rama2_[NombreApellido]`
Copia en `README.md` (o un fichero nuevo) una línea por cada entrada de `git log --oneline`. Por ejemplo:

```
## Información técnica añadida desde rama 2
f3a2b1c init: proyecto base SDAW_1917985
9d8e7f6 feat: añadir explicación de comandos en rama1
```

---

## Prompt sugerido para generar contenido con IA (requerido por la práctica)
> Genera un `README.md` completo para un proyecto Node.js llamado `SDAW_1917985`. El archivo debe incluir:
> - Descripción del proyecto.
> - Estructura de ficheros.
> - Instrucciones para instalar dependencias y arrancar el servidor.
> - Comandos Git usados durante la práctica con una breve explicación.
> - Capturas de pantalla (marcar el lugar donde se añadirán).
> - Conclusión personal.
>
> Proporciona además un archivo `server.js` usando Express que sirva `index.html` y un `index.html` con un botón que muestre "Hola Javier Díaz López".

---

## .gitignore sugerido
```
node_modules/
.env
.DS_Store
*.log
```


---
 
