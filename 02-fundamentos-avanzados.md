# 📌 Git: Fundamentos avanzados

## 🧩 Conceptos

- **HEAD:** apunta al último commit.
- **^:** último commit antes de la palabra o hash recién dado.
- **^n:** con n igual a la cantidad de commit anteriores.

##  modificaciones en los archivos

## Comandos diff

### Ver diferencia de archivos modificados con anteriores que no estan en el stage
```bash
git diff [archivo <opcional>]
```

### Ver diferencia de archivos modificados con anterior stage
```bash
git diff [archivo <opcional>] --staged
```

## Comandos commit

### actualizar mensaje del último commit realizado
```bash
git commit --amend -m "[Mensaje actualizado]"
```

### modo de edición del último commit realizado
```bash
git commit --amend
```

## Comandos reset

### resetea al commit anterior sin eliminar los cambios
```bash
git reset --soft [HEAD^ o hash]
```

### resetea al commit anterior sin eliminar los cambios ^n con n igual al numero de commits anteriores
```bash
git reset --soft [HEAD^{n} o hash]
```

### resetea el commit anterior y saca los cambios del stage
```bash
git reset --mixed [HEAD^ o hash]
```

### resetea el commit anterior y elimina todos los cambios, dejando todo a como estaba el commit especificado
```bash
git reset --hard [HEAD^ o hash]
```

## Comandos reflog

### log de la referencia de todo en orden cronologico
```bash
git reflog
```

## Comandos manejo de archivos

### comando para mover archivo especificado al path especificado, tambien se puede cambiar el nombre
```bash
git mv [file] [path o nuevo nombre]
```

### comando para remover archivo especificado
```bash
git rm [path/file]
```