# Indicadores de control y estándares de desempeño

## Enfoque

El control cierra el proceso administrativo: compara lo que ocurre con lo planeado y corrige los desvíos. Para el CRM se aplica en cuatro pasos:

1. **Establecer estándares:** se toman de las metas de la Entrega 2 (M1 a M5) y de las reglas del diccionario de datos (Entrega 3).
2. **Medir:** el propio CRM registra los datos; no se cargan planillas aparte.
3. **Comparar:** cada indicador tiene un responsable y una frecuencia de revisión.
4. **Corregir:** cada desvío tiene una acción prevista.

Se combinan tres momentos de control:

- **Preventivo:** reglas que impiden el error antes de que ocurra (por ejemplo, no guardar una oportunidad abierta sin próxima acción).
- **Concurrente:** alertas mientras el proceso ocurre (acciones vencidas).
- **Por retroalimentación:** revisión de resultados para ajustar el proceso (motivos de pérdida, conversión).

Los estándares marcados como **propuesto** no surgen de una meta aprobada: se validarán con la Gerencia Comercial. Los indicadores de negocio sin línea de base no tienen un estándar numérico inventado: se miden durante los dos primeros meses y el estándar se fija después.

## A. Indicadores de control del proceso comercial

| ID | Indicador | Fórmula | Estándar | Frecuencia y responsable | Acción ante el desvío |
|----|-----------|---------|----------|--------------------------|----------------------|
| IC-01 | Oportunidades abiertas con seguimiento completo | Abiertas con responsable, próxima acción y fecha / abiertas totales | 100 % (meta M3) | Control automático del CRM; revisión semanal del líder | Si el sistema permite un caso incompleto, se corrige la regla de validación. |
| IC-02 | Acciones vencidas | Abiertas con próxima acción vencida / abiertas totales | ≤ 10 % y ninguna con más de 7 días (propuesto) | Semanal, líder de Ventas | Reprogramar o reasignar en la reunión semanal. |
| IC-03 | Pérdidas con motivo registrado | Perdidas con motivo / perdidas totales | 100 % (regla del diccionario de datos) | Mensual, Gerencia Comercial | Completar el motivo con el vendedor y revisar las causas recurrentes. |
| IC-04 | Consultas digitales asignadas a tiempo | Consultas de redes asignadas dentro de 1 día hábil / recibidas | 100 % (propuesto) | Semanal, líder de Ventas | Revisar con la agencia la carga de consultas en el CRM. |
| IC-05 | Tasa de conversión | Oportunidades ganadas / oportunidades cerradas | Línea de base a medir en los primeros 2 meses | Mensual, Gerencia Comercial | Analizar la etapa del embudo donde se pierden más ventas. |
| IC-06 | Adopción del sistema | Vendedores con al menos una actividad por día hábil / vendedores activos | ≥ 90 % al terminar el piloto (propuesto) | Semanal, líder de Ventas | Acompañamiento y capacitación a quien no registra. |
| IC-07 | Tiempo de cierre | Días promedio entre la creación y el cierre de la oportunidad | Línea de base a medir en los primeros 2 meses | Mensual, Gerencia Comercial | Detectar etapas que demoran más de lo habitual. |

## B. Indicadores para la auditoría técnica del sistema

| ID | Indicador | Estándar | Cómo se verifica | Frecuencia |
|----|-----------|----------|------------------|------------|
| IT-01 | Rendimiento de las consultas habituales | 95 % en menos de 2 s con 10 usuarios simultáneos (meta M2) | Prueba de carga con al menos 200 consultas por tipo | Antes del piloto y en cada actualización mayor |
| IT-02 | Capacidad | 5.000 clientes y 20.000 actividades sin pérdida de registros (meta M1) | Carga de datos sintéticos y verificación de conteos y relaciones | Antes del piloto |
| IT-03 | Respaldos | 100 % de respaldos diarios exitosos y una restauración de prueba exitosa por mes | Registro de respaldos y restauración en un entorno separado | Diaria y mensual |
| IT-04 | Integridad de datos | 0 oportunidades sin cliente, 0 actividades sin autor, 0 CUIT duplicados | Consulta de control sobre la base | Mensual |
| IT-05 | Control de accesos | 100 % de usuarios con rol asignado; 0 cuentas activas de personas que dejaron la empresa | Revisión de la lista de usuarios contra el organigrama | Mensual |
| IT-06 | Disponibilidad | ≥ 99 % en horario laboral (propuesto) | Monitoreo del servidor | Mensual |
| IT-07 | Calidad de la importación desde el ERP | 100 % de registros con campos obligatorios; muestreo validado por el referente del ERP | Conteos, campos obligatorios y muestreo | En cada importación |

## Revisión de los indicadores

La revisión sigue la rutina propuesta para el área comercial:

| Quién | Qué revisa | Cuándo |
|-------|-----------|--------|
| Líder de Ventas | IC-01, IC-02, IC-04, IC-06 | Semanal |
| Gerencia Comercial | IC-03, IC-05, IC-07 | Mensual |
| Dirección | Resumen de IC-05 e IC-07, y estado de IT-03 a IT-06 | Mensual |
| Responsable técnico | IT-01 a IT-07 | Según la frecuencia de cada indicador |
