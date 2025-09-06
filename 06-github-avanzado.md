# 📌 Git: Github

## 🧩 Conceptos

- **Fork:** Un fork es una copia de un repositorio en tu propia cuenta de GitHub, que te permite experimentar con cambios sin afectar el proyecto original. Sirve para colaborar en proyectos de terceros.

- **Upstream:** Repositorio donde solo vas a traer información, Comunmente repositorio donde se hizo el fork.

- **Flujos de trabajo (Workflows):** Los flujos de trabajo en Git definen cómo un equipo organiza el uso de ramas, fusiones y PRs. Ejemplos comunes: Git Flow, GitHub Flow y Trunk-Based Development. Su objetivo es estandarizar cómo se integran los cambios al proyecto.

- **Feature Branch:** Una feature branch es una rama creada desde la principal (generalmente main o develop) para trabajar en una nueva funcionalidad de forma aislada. Una vez completada, se fusiona mediante PR.

- **Clone:** Clonar copia un repositorio remoto (el original o tu fork) a tu máquina, incluyendo su historial, para que trabajes localmente.

- **Workflows:** Los flujos de trabajo son la forma en que un equipo organiza cómo se crean, revisan y fusionan los cambios en el código. Estos definen reglas y pasos comunes, como trabajar en ramas para nuevas funciones o correcciones, crear pull requests para revisión, realizar pruebas automáticas y finalmente integrar los cambios en la rama principal, asegurando un proceso colaborativo ordenado y consistente.

- **Issues:** Los issues en GitHub son la principal herramienta para dar seguimiento a tareas, reportar errores, proponer nuevas funcionalidades o discutir ideas relacionadas con un proyecto. Funcionan como tickets que pueden asignarse, comentarse y priorizarse, lo que permite a los equipos organizar mejor el flujo de trabajo y centralizar la comunicación sobre aspectos específicos del desarrollo.

- **Labels:** Las labels son etiquetas de colores que se pueden aplicar a issues o pull requests para clasificarlos y facilitar su búsqueda y organización. Por ejemplo, se pueden usar para indicar la prioridad (alta, media, baja), el tipo de tarea (bug, feature, documentación), o el estado de un trabajo. Esto ayuda a mantener una visión clara y organizada del progreso del proyecto.

- **Milestones:** Los milestones permiten agrupar issues y pull requests bajo un mismo objetivo o entrega importante, como una versión del software. Funcionan como metas intermedias que ayudan a visualizar el progreso hacia un lanzamiento o hito específico. Cada milestone muestra el porcentaje de avance en función de las tareas completadas, lo que facilita medir el estado general del proyecto.

- **Colaboradores:** Los colaboradores en un repositorio de GitHub son las personas que tienen permisos de escritura y administración dentro de ese proyecto. Pueden contribuir directamente con código, gestionar issues, revisar y aprobar pull requests, entre otras tareas. Incluir colaboradores permite trabajar en equipo de manera más eficiente y aprovechar el control de versiones y la gestión de roles que ofrece GitHub.

- **Wiki:** Es una sección dentro de un repositorio de GitHub que permite documentar el proyecto de manera colaborativa, similar a una mini-enciclopedia, donde se pueden agregar guías, manuales de uso, procesos de instalación y cualquier información que ayude a los colaboradores o usuarios.

- **Proyectos:** Son tableros de gestión dentro de GitHub que permiten organizar tareas, issues y pull requests con metodologías como Kanban o Scrum, ayudando a planificar, priorizar y hacer seguimiento al progreso de un proyecto de desarrollo.

- **GitHub Pages:** Es una funcionalidad que permite desplegar páginas web estáticas directamente desde un repositorio, ideal para documentaciones, portafolios, blogs o demos de proyectos, utilizando ramas específicas o carpetas como fuente de publicación.

- **Insights:** Proporciona estadísticas y métricas sobre el repositorio, incluyendo la actividad de commits, contribuciones, tráfico, colaboradores y dependencias, lo que permite evaluar el estado, la salud y la evolución del proyecto.

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

## Comandos manejo de ramas e información de origin remoto

### comando para traer los cambios o ramas creadas en origin/remoto.
```bash
git pull --all
```

### comando para traer las referencias sin traer cambios o ramas creadas en origin/remoto.
```bash
git fetch -all
```

### comando para obtener todas las ramas disponibles, incluyendo las ramas del orgin/remoto.
```bash
git branch -all
```

### comando para revisar las ramas en el remoto y actualiza referencias.
```bash
git remote prune [origin]
```