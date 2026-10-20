# Git: control de versiones para proyectos

## Introducción

Git es un sistema de control de versiones. Permite registrar los cambios realizados en los archivos de un proyecto y consultar su historial. Así, podemos saber qué cambió, cuándo se hizo y quién lo hizo, además de recuperar versiones anteriores cuando sea necesario.

GitHub, en cambio, es una plataforma en línea donde se pueden alojar repositorios Git y colaborar con otras personas. Git funciona en el equipo local; GitHub facilita compartir y sincronizar el proyecto por Internet.

## ¿Cómo funciona Git?

Git guarda el historial del proyecto mediante **commits**, que son registros de un conjunto de cambios. Antes de crear un commit, se eligen los cambios que se quieren incluir. El proceso básico tiene tres partes:

1. **Directorio de trabajo:** carpeta donde se editan los archivos.
2. **Área de preparación (*staging area*):** espacio donde se seleccionan los cambios que formarán parte del siguiente registro.
3. **Repositorio:** historial local donde Git guarda los commits.

El flujo habitual es editar archivos, prepararlos y crear un commit. Cada commit incluye una descripción breve para identificar el cambio.

## Comandos básicos

Para iniciar Git en la carpeta de un proyecto:

```bash
git init
```

Para revisar los cambios y elegir qué archivos incluir:

```bash
git status
git add README.md
```

También se puede usar `git add .` para preparar todos los cambios de la carpeta actual. Después, se crea un commit:

```bash
git commit -m "Agrega la descripción del proyecto"
```

Para consultar el historial:

```bash
git log
```

## Git y GitHub en equipo

Cuando se conecta el repositorio local con uno alojado en GitHub, los cambios se pueden compartir:

- `git push` envía los commits locales al repositorio remoto.
- `git pull` obtiene cambios del repositorio remoto y los integra en la copia local.

Por ejemplo, después de crear un commit, se puede publicar con `git push`. Antes de comenzar a trabajar en un proyecto compartido, es recomendable ejecutar `git pull` para obtener los cambios recientes.

## ¿Por qué es útil?

- Mantiene un historial ordenado del proyecto.
- Permite comparar cambios y recuperar versiones anteriores.
- Facilita que varias personas colaboren sin intercambiar archivos manualmente.
- Ayuda a organizar el trabajo en ramas, que permiten desarrollar cambios por separado antes de integrarlos.

## Conclusión

Git ayuda a controlar la evolución de un proyecto mediante cambios registrados en commits. Al combinarlo con GitHub, también es posible guardar el repositorio en línea y colaborar con otras personas. Conocer comandos como `git status`, `git add`, `git commit`, `git pull` y `git push` proporciona una base para trabajar de manera organizada.
