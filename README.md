# CRM de Gestión Comercial para Caminiti Caminos S.A.

Trabajo Práctico Integrador y Progresivo · Organización Empresarial · Tecnicatura Universitaria en Programación a Distancia · Universidad Tecnológica Nacional.

## Descripción del sistema

Caminiti Caminos S.A. comercializa maquinaria agrícola y repuestos y brinda servicio técnico en campo en el noroeste de la provincia de Buenos Aires. Su identidad comercial se resume en una frase de su Dirección: *"no vende maquinaria; vende vínculos"*.

El relevamiento mostró que la historia de cada cliente, el seguimiento de las negociaciones y el conocimiento comercial quedan concentrados en las personas. El proyecto propone adaptar un **CRM de código abierto** que centralice clientes, oportunidades e interacciones, haga obligatorio el seguimiento de cada venta abierta y dé a la gerencia indicadores para decidir, sin reemplazar el trato personalizado.

Alcance de la primera versión: clientes, oportunidades por etapa, actividades y próxima acción, colaboración interna, panel de seguimiento y permisos por rol.

## Integrante

| Nombre | Rol | GitHub |
|--------|-----|--------|
| Mateo Sarco | Trabajo individual: análisis, diseño y documentación | [@Mateo0203s](https://github.com/Mateo0203s) |

Docente titular: Prof. Gabriela Martínez · Docente tutora: Monica Mut.

## Documentación

| Documento | Contenido |
|-----------|-----------|
| [Entrega 1](docs/entregas/entrega-1-organizacion-sistema-abierto.pdf) | La organización como sistema abierto y propuesta del CRM. |
| [Entrega 2](docs/entregas/entrega-2-diagnostico-y-planeacion.pdf) | FODA, objetivos, metas M1 a M5 y cronograma. |
| [Entrega 3](docs/entregas/entrega-3-estructura-formal-y-datos.pdf) | Organigrama y diccionario de datos. |
| [Proceso comercial (BPMN)](docs/01-proceso-comercial-bpmn.md) | Modelo BPMN 2.0 del proceso que el CRM transforma, con pools, lanes y compuertas. |
| [Historias de usuario](docs/02-historias-de-usuario.md) | HU-01 a HU-03 con criterios de aceptación y trazabilidad. |
| [Indicadores de control](docs/03-indicadores-de-control.md) | Indicadores del proceso, estándares de desempeño y auditoría técnica. |
| [Flujo de trabajo con Git](docs/04-flujo-de-trabajo-git.md) | Ramas, convención de commits y revisión de Pull Requests. |

## Gestión del proyecto

- **Tablero ágil:** [CRM Caminiti · Backlog](https://github.com/users/Mateo0203s/projects/1) (GitHub Projects), con las historias de usuario y sus estados *Por hacer*, *En progreso* y *Listo*.
- **Historias de usuario:** issues [#1](https://github.com/Mateo0203s/crm-caminiti-tpi/issues/1), [#2](https://github.com/Mateo0203s/crm-caminiti-tpi/issues/2) y [#3](https://github.com/Mateo0203s/crm-caminiti-tpi/issues/3).
- **Pull Requests:** cada documento se integró desde su propia rama mediante un [Pull Request revisado](https://github.com/Mateo0203s/crm-caminiti-tpi/pulls?q=is%3Apr). El trabajo es individual, por lo que la revisión es una autorrevisión formal con lista de control (ver [flujo de trabajo](docs/04-flujo-de-trabajo-git.md)).

## Declaración de uso de IA

### Herramienta y propósito

Se utilizó un asistente de Inteligencia Artificial Generativa (Claude, de Anthropic, en su entorno de programación Claude Code) como apoyo para estructurar los documentos, proponer borradores, modelar el diagrama BPMN, operar Git y GitHub desde la línea de comandos y revisar la redacción. Las entregas 1 y 2 incluyen su propia declaración de uso de IA.

El autor aportó toda la información sobre la empresa: la entrevista al propietario, el organigrama institucional, la forma real de trabajo del área comercial y las decisiones de alcance. La responsabilidad sobre la veracidad y la coherencia del trabajo es del estudiante.

### Prompts utilizados y su justificación

Los prompts se transcriben con la ortografía corregida.

| Prompt del autor | Para qué se usó | Por qué se formuló así |
|------------------|-----------------|------------------------|
| "Ahora falta la entrega 3, ¿cómo la continuamos y qué es lo que pide?" (adjuntando las entregas 1 y 2 y la consigna) | Interpretar la consigna y planificar la Entrega 3. | Dar las entregas previas como contexto obligaba a mantener la continuidad con el FODA, las metas y el alcance ya definidos, en lugar de empezar de cero. |
| "Ya tengo el organigrama" (adjuntando la foto del organigrama institucional) | Redibujar la estructura real con las convenciones normalizadas. | Se prefirió la fuente primaria de la empresa a cualquier estructura supuesta. |
| "El gerente comercial y el líder de ventas también cuentan como vendedores." | Corregir el análisis del tramo de control y del diccionario de datos. | El organigrama no muestra esa doble función; solo el autor la conocía. |
| "Tenemos que hacer lo que pide el TP4" (adjuntando la consigna) | Interpretar la Entrega 4 y planificar el BPMN, el repositorio, el tablero y los indicadores. | Se pidió primero la interpretación, para decidir el enfoque antes de producir contenido. |
| "Es individual, seguí así." | Resolver la revisión de pares en un trabajo individual. | Ante la imposibilidad técnica de aprobar el propio PR, se eligió una autorrevisión formal y declarada en lugar de simular un revisor. |

### Correcciones humanas sobre los resultados de la IA

1. **Organigrama.** La primera propuesta de la IA era una estructura hipotética: dividía Ventas por zonas geográficas y agregaba unidades que no existen. El autor la reemplazó por el organigrama real de la empresa, con dos gerencias, cuatro áreas y seis asesores externos. Como consecuencia, la división por zonas pasó a presentarse como un criterio informal de asignación y no como una unidad formal.
2. **Roles comerciales.** El autor corrigió que el gerente comercial y el líder de Ventas también venden, lo que modificó el tramo de control (seis personas que venden) y los responsables posibles de una cuenta en el diccionario de datos.
3. **Sucursal América y soporte externo.** El autor validó la ubicación de ambas unidades en el organigrama, que la IA había inferido de la foto, y aportó que la sucursal está en proceso de cierre.
4. **Formato.** La plantilla de la cátedra usa Calibri 12 con interlineado doble, pero la consigna de la Entrega 3 exige Arial 11 con interlineado 1,5. Se priorizó la consigna específica.
5. **Historias de usuario.** La consigna de la Entrega 4 menciona historias "previamente definidas", pero las entregas anteriores no las formulaban como tales. Se decidió definirlas en esta entrega y declararlo, en lugar de presentarlas como preexistentes.
6. **Estándares de desempeño.** Para la conversión y el tiempo de cierre no se aceptaron cifras sin fuente: quedan como indicadores a medir hasta contar con una línea de base. Los estándares sin respaldo en las metas aprobadas se marcan como propuestos.
7. **Revisión de Pull Requests.** Cada PR fue revisado contra la lista de control. En el PR del BPMN la revisión detectó que faltaba una guía de lectura de la notación, que se agregó antes de integrar.
