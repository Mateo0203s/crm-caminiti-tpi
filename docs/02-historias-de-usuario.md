# Historias de usuario

Las tres historias se definen en esta entrega a partir del alcance de la primera versión del CRM (Entrega 2) y del diccionario de datos (Entrega 3). Las entregas anteriores describían esas funciones, pero no las formulaban como historias de usuario.

Cada historia está registrada como *issue* y su estado se sigue en el tablero del proyecto (GitHub Projects).

## Estados del tablero

En esta etapa el proyecto está en diseño, por lo que los estados reflejan el **refinamiento** de cada historia, no su programación:

| Estado | Significado en esta etapa |
|--------|---------------------------|
| Por hacer | La historia está identificada en el backlog. |
| En progreso | Se están definiendo sus criterios de aceptación y su vínculo con el proceso y los indicadores. |
| Listo | Cumple la definición de listo: criterios de aceptación verificables, tareas BPMN asociadas, entidades de datos identificadas e indicador de control asignado. Queda preparada para el desarrollo (tareas T06 a T08 del cronograma). |

---

## HU-01 · Seguimiento obligatorio de oportunidades

**Como** vendedor, **quiero** registrar una próxima acción con fecha en cada oportunidad abierta, **para** no perder ventas por falta de seguimiento.

**Prioridad:** alta · **Meta asociada:** M3 (Entrega 2)

**Criterios de aceptación**

1. **Dado** una oportunidad en etapa distinta de *ganada* o *perdida*, **cuando** intento guardarla sin responsable, próxima acción o fecha, **entonces** el sistema rechaza el guardado e indica el dato faltante.
2. **Dado** una oportunidad abierta cuya fecha de próxima acción ya pasó, **cuando** abro mi panel, **entonces** la veo marcada como vencida.
3. **Dado** una oportunidad que pasa a *perdida*, **cuando** la guardo, **entonces** el sistema exige el motivo de pérdida.
4. Las oportunidades cerradas quedan exentas de la próxima acción.

**Trazabilidad:** BPMN, tareas *Registrar actividad y próxima acción* y *Rechazar el guardado*, compuerta *¿Responsable, acción y fecha completos?* · Entidad *Oportunidad* · Indicador IC-01.

---

## HU-02 · Historial compartido del cliente

**Como** vendedor, **quiero** consultar el historial completo de un cliente, **para** atenderlo con contexto aunque su vendedor habitual no esté.

**Prioridad:** alta · **Meta asociada:** M1 (Entrega 2)

**Criterios de aceptación**

1. **Dado** un cliente con actividades y oportunidades registradas, **cuando** abro su ficha, **entonces** veo sus oportunidades, las actividades ordenadas por fecha, el usado ofrecido y los comentarios internos.
2. **Dado** que no soy el responsable de la cuenta, **cuando** abro la ficha, **entonces** puedo consultarla pero no editar sus oportunidades.
3. **Dado** que registro una llamada a un cliente de otro vendedor, **cuando** la guardo, **entonces** queda en el historial con mi nombre como autor.

**Trazabilidad:** BPMN, tareas *Buscar cliente por CUIT o teléfono* y *Registrar actividad y próxima acción* · Entidades *Cliente* y *Actividad* · Indicadores IC-06 e IT-04.

---

## HU-03 · Panel de seguimiento comercial

**Como** líder o gerente comercial, **quiero** ver un panel con las oportunidades por etapa y por vendedor y las acciones vencidas, **para** intervenir a tiempo y proyectar las ventas.

**Prioridad:** media · **Meta asociada:** M2 (Entrega 2)

**Criterios de aceptación**

1. **Dado** oportunidades en distintas etapas, **cuando** abro el panel, **entonces** veo la cantidad y el importe estimado por etapa y por vendedor.
2. **Dado** acciones vencidas, **cuando** abro el panel, **entonces** las veo listadas con su responsable y los días de atraso.
3. **Dado** oportunidades cerradas en el mes, **cuando** filtro por período, **entonces** veo las ganadas, las perdidas y sus motivos.
4. Las consultas del panel responden en menos de 2 segundos en el 95 % de los casos con 10 usuarios simultáneos.

**Trazabilidad:** BPMN, tareas *Marcar acción vencida y alertar al líder*, *Revisar la vencida* y *Cerrar oportunidad y actualizar panel e indicadores* · Entidades *Oportunidad* y *Usuario* · Indicadores IC-02, IC-03 e IT-01.
