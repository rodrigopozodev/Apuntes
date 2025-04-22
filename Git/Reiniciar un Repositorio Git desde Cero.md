# 🧹 Reiniciar un Repositorio Git desde Cero

Este procedimiento elimina **todos los archivos y el historial de commits**, permitiéndote comenzar desde un estado completamente limpio. ⚠️ **Ten cuidado**: esto sobrescribe el historial anterior y no se puede deshacer si ya has hecho push sin backup.

---

## 🔧 Pasos para borrar todo y empezar de cero (manteniendo `.git`)

1. **Ir al directorio del repositorio**

```bash
cd /ruta/a/tu/repositorio
```

2. Eliminar todos los archivos y carpetas (menos .git)

```bash
rm -rf *
rm -rf .[^.]*  # elimina archivos ocultos, excepto .git
```

3. (Opcional) Crear un archivo inicial, por ejemplo un README

```bash
touch README.md
echo "# Nuevo inicio" > README.md
```

4. Añadir todos los archivos

```bash
git add .
```

5. Crear el nuevo commit inicial

```bash
git commit --allow-empty -m "Commit inicial desde cero"
```

6. Sobrescribir el repositorio remoto

```bash
git push -f origin main
```

## ❓ ¿Qué hace cada comando?

### rm -rf \*

- Elimina todos los archivos y carpetas visibles.

### rm -rf .[^.]\*

- Elimina archivos ocultos como .env, .vscode, etc., excepto .git.

### touch README.md

- Crea un archivo vacío README.md.

### git add .

- Añade todos los archivos al staging area.

### git commit --allow-empty

- Crea un nuevo commit, incluso si el directorio está vacío.

### git push -f origin main

- Fuerza la actualización del historial remoto con este nuevo inicio.
