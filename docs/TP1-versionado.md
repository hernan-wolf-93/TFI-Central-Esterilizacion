# TP N.º 1 — Versionado y Trabajo Colaborativo

## 1. Organización del repositorio

El proyecto utiliza Git como sistema de control de versiones y GitHub
como repositorio remoto.

La rama principal utilizada es `main`.

Para desarrollar tareas independientes se utilizaron ramas de
funcionalidad:

- `feature/documentacion`
- `feature/validacion-registros`

Esta organización permite separar los cambios y mantener estable
la rama principal.

## 2. Primera funcionalidad

La rama `feature/documentacion` tuvo como objetivo incorporar
documentación relacionada con el proceso de esterilización.

Se realizaron dos commits:

- `docs: agregar descripción del proceso de esterilización`
- `docs: especificar datos de trazabilidad del proceso`

## 3. Segunda funcionalidad

La rama `feature/validacion-registros` tuvo como objetivo documentar
las validaciones de los registros del sistema.

Se realizaron dos commits:

- `docs: agregar validaciones iniciales de registros`
- `docs: documentar resultados del procesamiento`

## 4. Conflicto de fusión

Para provocar un conflicto controlado se modificó la misma sección
del archivo `docs/proceso-esterilizacion.md` desde dos ramas diferentes.

Las modificaciones fueron incompatibles entre sí y Git no pudo
resolver automáticamente la fusión.

## 5. Resolución

Se analizaron ambas versiones y se decidió combinar la información
relevante de cada una.

La versión final mantiene la identificación del instrumental, la
preparación de la bandeja, el procesamiento mediante autoclave,
el control del resultado y la trazabilidad.

El conflicto fue resuelto manualmente y posteriormente se creó un
commit específico para registrar la resolución.

## 6. Pull Request

Se creó un Pull Request desde `feature/documentacion` hacia `main`.

Se realizó una revisión de los cambios y se verificó que la
documentación correspondiera al objetivo de la rama antes de realizar
el merge.