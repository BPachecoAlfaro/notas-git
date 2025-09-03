# 📌 Git: Github

## 🧩 Conceptos

- **Fork:** Un fork es una copia de un repositorio en tu propia cuenta de GitHub, que te permite experimentar con cambios sin afectar el proyecto original. Sirve para colaborar en proyectos de terceros.

- **Upstream:** Repositorio donde solo vas a traer información, Comunmente repositorio donde se hizo el fork.

- **Flujos de trabajo (Workflows):** Los flujos de trabajo en Git definen cómo un equipo organiza el uso de ramas, fusiones y PRs. Ejemplos comunes: Git Flow, GitHub Flow y Trunk-Based Development. Su objetivo es estandarizar cómo se integran los cambios al proyecto.

- **Feature Branch:** Una feature branch es una rama creada desde la principal (generalmente main o develop) para trabajar en una nueva funcionalidad de forma aislada. Una vez completada, se fusiona mediante PR.

- **Clone:** Clonar copia un repositorio remoto (el original o tu fork) a tu máquina, incluyendo su historial, para que trabajes localmente.

- **Workflows:** Los flujos de trabajo son la forma en que un equipo organiza cómo se crean, revisan y fusionan los cambios en el código. Estos definen reglas y pasos comunes, como trabajar en ramas para nuevas funciones o correcciones, crear pull requests para revisión, realizar pruebas automáticas y finalmente integrar los cambios en la rama principal, asegurando un proceso colaborativo ordenado y consistente.

##  Comandos github avanzado

## Comandos clone

### Clonar repositorio remoto a tu computadora.
```bash
git clone [url-rep]
```

## Comandos fork

### Conectar con el repo original.
```bash
git remote add upstream [url-original]
```

### Conectar con el repo original.
```bash
git remote add upstream <url-original>
```

### Obtener cambios del original.
```bash
git fetch upstream
```

### Comandos branch

### Subir rama al repositorio remoto
```bash
git push --set-upstream [origin o nombre del origen remoto] [Nombre rama a subir]
```