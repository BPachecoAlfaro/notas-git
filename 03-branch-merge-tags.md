# 📌 Git: ramas, merge y tags

## 🧩 Conceptos

- **Branch:** Una rama es una línea de desarrollo independiente dentro de un repositorio Git. Sirve para trabajar en nuevas funcionalidades, corregir errores o experimentar sin afectar directamente a la rama principal.
- **Merge:** El merge es la acción de combinar los cambios de una rama en otra. Generalmente se usa para llevar los cambios de una rama de desarrollo a la rama principal.
- **Merge fast-forward:** Este tipo de merge ocurre cuando la rama destino no tiene commits nuevos desde que se creó la rama que se quiere integrar. En este caso, Git simplemente “mueve el puntero” de la rama destino hasta el último commit de la rama origen, sin necesidad de crear un nuevo commit de merge. Es el escenario más simple y limpio.

##  Comandos de ramas y merge

## Comandos branch

### Crear una nueva rama
```bash
git branch [nombre nueva rama]
```

### Cambiar a una rama en especifico
```bash
git checkout [nombre de rama]
```

### Eliminar una rama
```bash
git branch -d [nombre de rama]
```
```bash
git branch -d [nombre de rama] -f # De manera forzada
```

## Comandos Merge

### Traer cambios desde la rama especificada a la actual
```bash
git merge [nombre rama]
```