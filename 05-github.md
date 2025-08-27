# 📌 Git: Github

## 🧩 Conceptos

- **Repositorio:** Un repositorio en GitHub es el espacio donde se almacena el código fuente y su historial de versiones, junto con documentación, issues y configuraciones. Puede ser público (visible para todos) o privado (solo accesible para colaboradores autorizados). Es la unidad central de trabajo en GitHub.

- **Fork:** Un fork es una copia de un repositorio que se crea en tu cuenta de GitHub para poder modificarlo libremente sin afectar el original. Se usa comúnmente para contribuir a proyectos de terceros: haces cambios en tu fork y luego envías un pull request al repositorio original.

- **Pull Request (PR):** Un pull request es la forma en que se proponen cambios a un repositorio. Permite discutir, revisar y aprobar modificaciones antes de que se integren a la rama principal. Es una herramienta clave para la colaboración en proyectos de código abierto o en equipos de desarrollo.

- **Issue:** Los issues son tickets o reportes que sirven para dar seguimiento a errores, nuevas funcionalidades, dudas o tareas pendientes dentro de un proyecto. Se pueden asignar a personas, etiquetar y vincular con pull requests para mantener la trazabilidad del trabajo.

- **Actions (GitHub Actions):** GitHub Actions es una herramienta de integración y entrega continua (CI/CD) que permite automatizar flujos de trabajo directamente en GitHub, como ejecutar pruebas, compilar el código o desplegar aplicaciones cuando se hacen commits o PRs.

##  Comandos para repositorio remoto

## Comandos básicos

### Agregar un origen remoto
```bash
git remote add [origin por estandar - nombre repositorio a gusto] [url github]
```

### Revisar las fuentes remotas de nuestro repositorio.
```bash
git remote -v
```

### Hacer un push a un repositorio.
```bash
git push -u [origin por estandar - nombre repositorio] [master - rama que deseamos enviar]
```
> [!NOTE]
> -u: Nos ayuda a que la próxima vez que queramos hacer push, no necesitemos especificar la rama y el origin. Setea uno por defecto

### Hacer push de los tags.
```bash
git push --tags
```

### Hacer un pull de un repositorio.
```bash
git pull [origin por estandar - nombre repositorio <opcional>] [master - rama que deseamos recibir<opcional>]
```
> [!NOTE]
> -u: al haber realizado el git push -u, establece por defecto el nombre del repositorio y la rama.