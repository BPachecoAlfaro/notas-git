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

### actualizar mensaje del ultimo commit realizado
```bash
git commit --amend -m "[Mensaje actualizado]"
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