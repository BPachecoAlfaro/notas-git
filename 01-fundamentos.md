# 📌 Git: Fundamentos

##  ¿Qué es Git?

- **Git** es un **sistema de control de versiones distribuido**.
- Permite llevar el historial de cambios de un proyecto (código, documentos, etc.).
- Fue creado por **Linus Torvalds** en 2005 para el desarrollo del kernel de Linux.

👉 **Idea clave**: Git es como una _máquina del tiempo_ para tus archivos.


## 🔑 Diferencia entre Git y GitHub

- **Git**: herramienta de control de versiones (instalada en tu PC).
- **GitHub/GitLab/Bitbucket**: plataformas en la nube para alojar repositorios y colaborar.

| Git (local)                  | GitHub/GitLab (remoto)                |
| ---------------------------- | ------------------------------------- |
| Maneja tu historial en tu PC | Guarda y comparte repositorios online |
| No necesita internet         | Necesita internet                     |
| Herramienta                  | Servicio basado en Git                |



## 🧩 Conceptos básicos

- **Repositorio (repo):** carpeta con historial de versiones.
- **Commit:** un “punto de guardado” con los cambios registrados.
- **Branch (rama):** línea de desarrollo independiente.
- **Staging area (índice):** espacio temporal donde preparas los cambios antes de confirmarlos.
- **HEAD:** puntero al commit actual en el que estás trabajando.



## 📂 Flujo general de trabajo con Git

1. Modificar archivos en el **working directory**.
2. Añadir cambios al **staging area** (`git add`).
3. Confirmar cambios con un **commit** (`git commit`).
4. (Opcional) Subirlos a un **repositorio remoto** (`git push`).

```txt
[Working Directory] → git add → [Staging Area] → git commit → [Local Repo] → git push → [Remote Repo]
```



## Comandos básicos

### Ver versión de Git
```bash
git --version
```
### Comando de ayuda
```bash
git help
```
### Comando de ayuda de comando
```bash
git help [comando]
```
### Comando de configuracion de user
```bash
git config --global user.name "[UserName]"
git config --global user.email "[UserEmail]"
```
### Comando de configuracion de rama principal
```bash
git config --global init.defaultBranch <name>
```
### Comando sobre commits, rama donde estas trabajando
```bash
git status
```

### Comando para cambiar nombre de la rama
```bash
git branch -m [nombre de la rama] [nuevo nombre]
```

## Comandos principales

### Comando de inicialización de repositorio
```bash
git init
```

### Comando para iniciar el seguimiento de archivo o directorio
```bash
git add [archivo o directorio]
```

### Comando para remover el seguimiento de archivo o directorio
```bash
git reset [archivo o directorio]
```

### Comando para agregar al stage el archivo o directorio
```bash
git commit [-m o --message] ["Mensaje del commit"]
```

### Comando para recuperar estado del commit anterior
```bash
git checkout -- [archivo o directorio]
```
> [!NOTE]
> "--" Do not interpret any more arguments as options.

### Comando para agregar al stage y realizar commit
```bash
git commit -am ["Mensaje del commit"]
```
> [!NOTE]
> Solo funciona si el archivo ya se encuentra en seguimiento.

### Comando visualizar para los registros de los commits realizados
```bash
git log
```

### Comando agregar al stage archivos que hacen match
```bash
git add *.[tipo de archivo]
```

### Comando agregar al stage archivos que hacen match dentro de un directorio especifico
```bash
git add [directorio]*.[tipo de archivo]
```

### Comando agregar al stage un directorio y subcarpetas y/o archivos
```bash
git add [directorio]/
```

### Git no hace seguimientos de directorio vacios por lo que hay que especificar que se necesita hacer el seguimiento creando un archivo .gitkeep
```bash
[directorio]/.gitkeep
```
