# 🧹 Reiniciar un Repositorio Git desde Cero

Este procedimiento elimina **todo el historial de commits** y te permite comenzar con un **nuevo commit inicial limpio**. ⚠️ **Ten cuidado**: esto es irreversible si ya has hecho push a un repositorio remoto sin backup.

---

## 🔧 Pasos para reiniciar el historial de Git

1. **Ir al directorio del repositorio**

```bash
cd /ruta/a/tu/repositorio
```

2. Crear una nueva rama sin historial (rama "huérfana")

```bash
git checkout --orphan nueva-rama
```

3. Añadir todos los archivos al nuevo commit

```bash
git add .
```

4. Crear el nuevo commit inicial

```bash
git commit -m "Commit inicial limpio"
```

5. Eliminar la rama principal anterior (por ejemplo, main)

```bash
git branch -D main
```

6. Renombrar la nueva rama a main

```bash
git branch -m main
```

7. Sobrescribir el repositorio remoto (si ya existe)

```bash
git push -f origin main
```

## ❓ ¿Qué hace cada comando?

**git checkout --orphan nueva-rama**

- Crea una nueva rama sin historial previo.

**git add .**

- Añade todos los archivos al staging area.

**git commit -m "..."**

- Crea el nuevo commit inicial.

**git branch -D main**

- Elimina la antigua rama main localmente.

**git branch -m main**

- Renombra la rama actual a main.

**git push -f origin main**

- Fuerza la actualización del repositorio remoto (⚠️ ¡esto sobrescribe la historia anterior!).
