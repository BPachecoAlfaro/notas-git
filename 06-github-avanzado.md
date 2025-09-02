# 📌 Git: Github

## 🧩 Conceptos

- **Fork:** Un fork es una copia de un repositorio en tu propia cuenta de GitHub, que te permite experimentar con cambios sin afectar el proyecto original. Sirve para colaborar en proyectos de terceros.

- **Upstream:** Repositorio donde solo vas a traer información, Comunmente repositorio donde se hizo el fork.

- **Flujos de trabajo (Workflows):** Los flujos de trabajo en Git definen cómo un equipo organiza el uso de ramas, fusiones y PRs. Ejemplos comunes: Git Flow, GitHub Flow y Trunk-Based Development. Su objetivo es estandarizar cómo se integran los cambios al proyecto.

- **Feature Branch:** Una feature branch es una rama creada desde la principal (generalmente main o develop) para trabajar en una nueva funcionalidad de forma aislada. Una vez completada, se fusiona mediante PR.
👉 Comandos útiles:

- **Clone:** Clonar copia un repositorio remoto (el original o tu fork) a tu máquina, incluyendo su historial, para que trabajes localmente.

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
git fetch upstream  
```

### Obtener cambios del original.
```bash
git remote add upstream <url-original>
```
git merge upstream/main    # Integrar cambios