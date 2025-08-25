# 📌 Git: stash, rebase

## 🧩 Conceptos

- **Stash:** permite guardar cambios locales de forma temporal sin hacer commit, ideal para cambiar de rama o actualizar el proyecto sin perder trabajo.
- **Rebase:** reescribe la historia de commits aplicando los cambios de una rama sobre otra, generando un historial más lineal y claro.

##  Comandos de stash y rebase

## Comandos stash

### Guarda los cambios pendientes en un área temporal.
```bash
git stash
```

### Guarda también los archivos no rastreados (untracked).
```bash
git stash -u
```

### Muestra los stashes guardados
```bash
git git stash list
```

### Aplica un stash y lo elimina de la lista. Específico si agregas el id.
```bash
git stash pop [optional <id>]
```

### Aplica un stash sin borrarlo por defecto el últimos. Específico si agregas el id.
```bash
git stash apply [optional <id>]
```

### Elimina todos los stashes guardados.
```bash
git stash clear
```

### Guarda el stash con un mensaje.
```bash
git stash save ["mensaje"]
```

### Crea una nueva rama desde donde se hizo el stash y aplica esos cambios allí. Específico si agregas el id.
```bash
git stash branch [nombre-rama] [optional <id>]
```