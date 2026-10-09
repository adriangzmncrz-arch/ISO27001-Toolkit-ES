# Procedimiento de No Conformidades y Acciones Correctivas

| Campo | Valor |
|---|---|
| Código | PRO-05 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | 10.1, 10.2 |

> 💡 **Cómo adaptar:** el error más frecuente que encuentran los auditores es confundir **corrección** con **acción correctiva**. Revocar el acceso olvidado es la corrección; cambiar el proceso para que RR. HH. notifique automáticamente las bajas es la acción correctiva.

## 1. Propósito

Reaccionar ante las no conformidades, eliminar sus causas para evitar que se repitan y mejorar continuamente el SGSI.

## 2. Fuentes de no conformidades

- Auditorías internas y externas.
- Incidentes de seguridad.
- Revisión por la dirección.
- Seguimiento de objetivos e indicadores.
- Pruebas de controles (respaldos, accesos, continuidad).
- Quejas de clientes o partes interesadas.
- Detección por cualquier colaborador.

## 3. Proceso

| Paso | Actividad | Responsable | Plazo |
|---|---|---|---|
| 1 | Registrar la no conformidad en REG-06 con su descripción y evidencia | Quien la detecta / Responsable del SGSI | Al detectarla |
| 2 | **Corrección:** controlar y corregir el efecto inmediato | Responsable del proceso | Lo antes posible |
| 3 | **Análisis de causa raíz** | Responsable del proceso con apoyo del Responsable del SGSI | [10] días hábiles |
| 4 | Determinar si existen o podrían ocurrir no conformidades similares en otros procesos | Responsable del SGSI | Con el paso 3 |
| 5 | Definir e implementar la **acción correctiva** | Responsable del proceso | Según el plan; mayores en ≤ [60] días, menores en ≤ [90] días |
| 6 | **Verificar la eficacia** | Responsable del SGSI o auditor | [30-90] días después de implementar |
| 7 | Cerrar o reabrir; actualizar riesgos o el SGSI si es necesario | Responsable del SGSI | Tras la verificación |

## 4. Análisis de causa raíz

Se recomienda alguna de estas técnicas, según la complejidad:

**Cinco porqués** (problemas simples)
> *No conformidad:* un excolaborador conservó acceso al CRM durante 20 días.
> 1. ¿Por qué? TI no deshabilitó la cuenta del CRM.
> 2. ¿Por qué? TI no sabía que la persona había salido.
> 3. ¿Por qué? RR. HH. avisó por correo a una persona de TI que estaba de vacaciones.
> 4. ¿Por qué? No existe un canal definido para notificar bajas.
> 5. ¿Por qué? El procedimiento de bajas no estaba documentado.
>
> *Causa raíz:* proceso de bajas no definido. *Acción correctiva:* implementar PRO-07 con solicitud por ticket a una cola de TI y revisión semanal cruzada RR. HH.–TI.

**Diagrama de Ishikawa** (problemas con varias causas posibles): personas, procesos, tecnología, proveedores, entorno y medición.

## 5. Verificación de eficacia

Una acción correctiva es eficaz cuando la evidencia demuestra que **la no conformidad no se ha repetido** en un periodo razonable o en una muestra representativa. Haber implementado la acción no basta para cerrarla.

## 6. Mejora continua (10.1)

Las oportunidades de mejora identificadas en auditorías, revisiones, incidentes y sugerencias del personal se registran en REG-06 con tipo "Mejora" y se priorizan en el Comité de Seguridad.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
