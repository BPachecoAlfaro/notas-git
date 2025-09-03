# 📌 Git: ramas, merge y tags

## 🧩 Conceptos

- **Branch:** Una rama es una línea de desarrollo independiente dentro de un repositorio Git. Sirve para trabajar en nuevas funcionalidades, corregir errores o experimentar sin afectar directamente a la rama principal.
- **Merge:** El merge es la acción de combinar los cambios de una rama en otra. Generalmente se usa para llevar los cambios de una rama de desarrollo a la rama principal.
- **Merge fast-forward:** Este tipo de merge ocurre cuando la rama destino no tiene commits nuevos desde que se creó la rama que se quiere integrar. En este caso, Git simplemente “mueve el puntero” de la rama destino hasta el último commit de la rama origen, sin necesidad de crear un nuevo commit de merge. Es el escenario más simple y limpio.
- **Merge automatico:** Aquí ambas ramas han avanzado de forma independiente, pero sus cambios no interfieren entre sí (por ejemplo, modificaron archivos o líneas distintas). Git puede combinar las dos historias automáticamente y crea un commit de merge que une los cambios, sin necesidad de intervención manual.
- **Merge con conflictos:** Se da cuando las ramas han modificado las mismas líneas de un archivo o una rama eliminó un archivo que la otra modificó. En este caso, Git no puede decidir qué versión conservar, por lo que marca un conflicto. El desarrollador debe revisar los archivos conflictivos, elegir o combinar los cambios y luego confirmar el merge manualmente.
- **Merge abortado:** Si durante el proceso de merge surgen conflictos y se decide no resolverlos en ese momento, Git permite abortar la operación. Esto devuelve la rama al estado previo al intento de fusión, dejando el historial limpio y sin cambios aplicados, como si el merge nunca hubiera ocurrido.
- **Merge squash:** Aunque no es un merge tradicional, se utiliza mucho para mantener un historial más ordenado. Este proceso toma todos los commits de una rama y los combina en un único commit antes de integrarlos en la rama destino. Es útil cuando se quiere que el historial muestre un solo commit representativo en lugar de muchos pequeños.
- **Tag:** Un tag en Git es una etiqueta que apunta a un commit específico en la historia del repositorio, usada principalmente para marcar versiones o hitos importantes del proyecto. A diferencia de una rama, un tag no cambia ni avanza: siempre queda fijo en ese commit, lo que lo hace ideal para identificar releases estables.

##  Comandos de ramas y merge

## Comandos branch

### Crear una nueva rama
```bash
git branch [nombre nueva rama]
```

### Crear una nueva rama y cambiarse a ella
```bash
git checkout -b [nombre nueva rama]
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

### Para cancelar un merge en curso
```bash
git merge --abort
```

### Para combinar todos los commits de una rama en un solo commit antes de integrarlo
```bash
git merge --squash [nombre rama merge]
git commit -m "[Mensaje commit representativo]"
```

## Comandos Tags

### Ver todos los tags del repositorio
```bash
git tag
```

### Crear un tag simple 
```bash
git tag [nombre del tag] [hash commit o HEAD<optional>]
```

### Crear un tag anotado
```bash
git tag -a [nombre del tag] [hash commit o HEAD<optional>] -m "[mensaje tag]"
```
> [!NOTE]
> Si no se proporciona el hash o HEAD, toma por defecto el actual commit

### Eliminar un tag
```bash
git tag -d [nombre del tag a eliminar]
```

### Mostrar información detallada de un tag anotado
```bash
git show [nombre del tag]
```