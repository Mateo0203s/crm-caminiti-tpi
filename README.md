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

Se transcriben los prompts efectivamente utilizados, en orden cronológico, de forma fiel: con la ortografía corregida y los nombres de personas reemplazados por cargos. Para cada uno se indica el contexto aportado, qué devolvió la IA y qué decidió el autor.

#### Entrega 3: estructura formal y diseño de datos

| # | Prompt del autor | Contexto aportado | Qué devolvió la IA | Evaluación crítica y decisión del autor |
|---|------------------|-------------------|--------------------|------------------------------------------|
| 1 | "Ahora falta la Entrega 3, ¿cómo la continuamos? ¿Qué es lo que pide?" | Entregas 1 y 2 y la consigna de la Entrega 3. | Interpretación de la consigna. Propuesta de representar a toda la empresa y no un área de sistemas, porque esa área no existe. Primer esquema del diccionario de datos a partir del alcance de la Entrega 2. | Se aceptó representar la empresa completa. Se decidió no presentar ninguna estructura sin validarla antes con el propietario. |
| 2 | "Comencemos a armar, que a la tarde me junto con el dueño." | Reunión pendiente con el propietario. | Un borrador completo con todas las hipótesis resaltadas en amarillo y una lista de 13 preguntas para la reunión. | El borrador se usó solo como guía de la entrevista. Ningún dato resaltado se entregó sin confirmar. |
| 3 | "Me faltó pasarte esto." | Plantilla de entregas de la cátedra (.docx). | Adaptación del documento a la estructura de la plantilla y detección de un conflicto: la plantilla usa Calibri 12 con interlineado doble y la consigna pide Arial 11 con 1,5. | Se priorizó la consigna específica de la entrega y se conservó la estructura de la plantilla. |
| 4 | "Ya tengo el organigrama." | Foto del organigrama institucional de la empresa. | Organigrama redibujado con convenciones normalizadas (rectángulos, cargos en lugar de nombres, staff con líneas de trazos) y un análisis nuevo: la venta y el stock dependen de gerencias distintas. | Se descartó por completo la estructura hipotética del borrador. El autor verificó las dos interpretaciones dudosas de la foto: la ubicación de Sucursal América y la del soporte externo. |
| 5 | "El gerente comercial y el líder de Ventas también cuentan como vendedores. Lo de la sucursal, que va a cerrar, dejémoslo así. Lo del soporte externo está bien. ¿Está para entregar?" | Conocimiento directo del funcionamiento del área comercial. | Actualización del tramo de control (6 personas que venden) y de los responsables posibles de una cuenta en el diccionario de datos. | Era una información que el organigrama no mostraba y solo el autor conocía. Con ella se confirmó el rango de 5 a 7 usuarios estimado en la Entrega 2. |

#### Adopción del sistema en la empresa (trabajo complementario a las entregas)

| # | Prompt del autor | Contexto aportado | Qué devolvió la IA | Evaluación crítica y decisión del autor |
|---|------------------|-------------------|--------------------|------------------------------------------|
| 6 | "Quiero una presentación educativa para el equipo comercial: demostrarles por qué deben usar un CRM, para qué sirve, cómo se usa y qué beneficios tiene, con ejemplos reales." | Las entregas anteriores y la percepción del autor sobre el área de ventas. | Una presentación de 17 diapositivas con casos basados en el relevamiento y una advertencia: un tono descalificador hacia el equipo aumentaría el riesgo de baja adopción (amenaza A1). | Se aceptó el enfoque respetuoso. Los casos se presentaron como situaciones típicas, sin estadísticas inventadas. |
| 7 | "¿Qué más se le podría ofrecer más allá del CRM? Puedo tener acceso de lectura a la base de datos del ERP." | Posible acceso de solo lectura al ERP. | Propuestas de tablero de gestión, análisis de stock de repuestos y oportunidades a partir de las compras, con advertencias sobre la autorización escrita, el proveedor del ERP y la Ley 25.326 de protección de datos personales. | Se priorizaron el tablero y el análisis de stock como primera etapa de bajo riesgo. Las advertencias se reflejan en el acceso de solo lectura y en el indicador IT-07. |
| 8 | "Armame una presentación para ir a hablar con la Dirección y vender la propuesta." | El diagnóstico y el plan de las entregas. | Una propuesta de 16 diapositivas con tres pilares, plan por etapas e inversión, con los montos como marcadores vacíos. | Se mantuvieron los montos vacíos: los completa el autor con datos reales, y no se aceptaron cifras inventadas. |
| 9 | "La idea es que la primera charla sea educativa y que ellos mismos se den cuenta de que necesitan un CRM, no que yo se los venda." | Decisión del autor sobre la estrategia de cambio. | Un taller de 14 diapositivas con ejercicios y un autodiagnóstico, donde el término CRM aparece recién al final. | Fue una corrección de enfoque del autor: pasar de vender la herramienta a que el equipo descubra la necesidad, como estrategia de gestión del cambio frente a la amenaza A1. |

#### Entrega 4: procesos, trabajo colaborativo y control

| # | Prompt del autor | Contexto aportado | Qué devolvió la IA | Evaluación crítica y decisión del autor |
|---|------------------|-------------------|--------------------|------------------------------------------|
| 10 | "Tenemos que hacer lo que pide el TP4." | Consigna de la Entrega 4. | Interpretación de las cuatro consignas y dos alertas: las historias de usuario no estaban definidas en las entregas previas, y la revisión de pares requiere otra persona. | Se decidió definir las historias en esta entrega y declararlo, en lugar de presentarlas como preexistentes. |
| 11 | "Es individual, seguí así." | El trabajo práctico es individual. | Propuesta de autorrevisión formal: plantilla de PR con lista de control, comentario de revisión y correcciones antes de integrar. | Se eligió declarar la autorrevisión en lugar de simular un revisor externo. |
| 12 | "Sí, con los PDF." | Respuesta a la consulta de la IA antes de publicar el repositorio. | Antes de publicar, la IA detalló qué quedaría público (entregas con la síntesis de la entrevista y el organigrama por cargos) y pidió autorización. | El autor autorizó la publicación; el organigrama ya no incluía nombres de personas. |

### Patrones observados en el uso de la IA

- **Completa vacíos con hipótesis verosímiles.** El primer organigrama dividía Ventas por zonas y agregaba unidades inexistentes. Control aplicado: marcar toda hipótesis como tal y validarla con la fuente primaria antes de entregarla.
- **Propone estructuras de manual.** El valor del análisis apareció al contrastar esas estructuras con los datos reales de la empresa, como el hallazgo de las dos cadenas de mando.
- **No se aceptaron cifras sin fuente:** ni estándares de desempeño, ni montos de inversión, ni estadísticas en las presentaciones.
- **Rinde en tareas instrumentales** (formato, maquetación, BPMN, Git y GitHub), pero cada resultado se verificó: el modelo BPMN con un script, los enlaces del README y la maquetación de cada PDF.
- **Las decisiones fueron del autor:** el alcance, el enfoque de cada entrega, el tono hacia la empresa y la publicación del repositorio.

### Correcciones humanas sobre los resultados de la IA

1. **Organigrama.** La primera propuesta de la IA era una estructura hipotética: dividía Ventas por zonas geográficas y agregaba unidades que no existen. El autor la reemplazó por el organigrama real de la empresa, con dos gerencias, cuatro áreas y seis asesores externos. Como consecuencia, la división por zonas pasó a presentarse como un criterio informal de asignación y no como una unidad formal.
2. **Roles comerciales.** El autor corrigió que el gerente comercial y el líder de Ventas también venden, lo que modificó el tramo de control (seis personas que venden) y los responsables posibles de una cuenta en el diccionario de datos.
3. **Sucursal América y soporte externo.** El autor validó la ubicación de ambas unidades en el organigrama, que la IA había inferido de la foto, y aportó que la sucursal está en proceso de cierre.
4. **Formato.** La plantilla de la cátedra usa Calibri 12 con interlineado doble, pero la consigna de la Entrega 3 exige Arial 11 con interlineado 1,5. Se priorizó la consigna específica.
5. **Historias de usuario.** La consigna de la Entrega 4 menciona historias "previamente definidas", pero las entregas anteriores no las formulaban como tales. Se decidió definirlas en esta entrega y declararlo, en lugar de presentarlas como preexistentes.
6. **Estándares de desempeño.** Para la conversión y el tiempo de cierre no se aceptaron cifras sin fuente: quedan como indicadores a medir hasta contar con una línea de base. Los estándares sin respaldo en las metas aprobadas se marcan como propuestos.
7. **Revisión de Pull Requests.** Cada PR fue revisado contra la lista de control. En el PR del BPMN la revisión detectó que faltaba una guía de lectura de la notación, que se agregó antes de integrar.
