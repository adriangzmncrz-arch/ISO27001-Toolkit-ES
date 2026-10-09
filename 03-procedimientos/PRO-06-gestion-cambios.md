# Procedimiento de Gestión de Cambios

| Campo | Valor |
|---|---|
| Código | PRO-06 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DE TI] |
| Aprobó | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | 6.3, A.8.32, A.8.9, A.8.19 |

> 💡 **Cómo adaptar:** el objetivo es controlar el riesgo, no frenar la operación. Define una lista de cambios estándar preaprobados (por ejemplo, alta de usuario, despliegue automatizado con pruebas superadas) para que solo los cambios con riesgo real pasen por aprobación.

## 1. Propósito

Asegurar que los cambios a sistemas, infraestructura, aplicaciones y servicios de información se evalúen, aprueben, prueben e implementen de forma controlada.

## 2. Alcance

Cambios en producción a servidores, redes, servicios en la nube, aplicaciones, bases de datos, configuraciones de seguridad y servicios de proveedores que afecten el alcance del SGSI.

## 3. Tipos de cambio

| Tipo | Descripción | Aprobación | Ejemplos |
|---|---|---|---|
| **Estándar** | Repetitivo, de bajo riesgo, con procedimiento probado | Preaprobado; solo se registra | Alta de usuario, parche mensual de equipos de usuario, despliegue por *pipeline* con pruebas superadas |
| **Normal** | Requiere evaluación de riesgo e impacto | Responsable de TI; si es de alto riesgo, también el Responsable del SGSI | Cambio de reglas de firewall, migración de base de datos, nueva integración |
| **Emergencia** | Necesario para restablecer un servicio o corregir una vulnerabilidad crítica | Aprobación verbal de [ROL], registro posterior en ≤ [1] día hábil | Parche de día cero, restauración tras un incidente |

## 4. Flujo de un cambio normal

| Paso | Actividad | Responsable |
|---|---|---|
| 1 | Registrar la solicitud en [HERRAMIENTA] con descripción, justificación, sistemas afectados, ventana propuesta | Solicitante |
| 2 | Evaluar impacto en seguridad, disponibilidad y riesgos; definir plan de pruebas y de reversión | Implementador |
| 3 | Aprobar | Ver tabla 3 |
| 4 | Probar en ambiente no productivo cuando exista | Implementador |
| 5 | Comunicar a usuarios afectados | Implementador |
| 6 | Implementar en la ventana acordada | Implementador |
| 7 | Verificar resultado; aplicar reversión si falla | Implementador |
| 8 | Cerrar el registro y actualizar documentación, inventario y diagramas | Implementador |

## 5. Contenido mínimo del registro

- Identificador, solicitante, fecha.
- Descripción y justificación.
- Sistemas y servicios afectados.
- Evaluación de riesgo e impacto.
- Plan de pruebas y de reversión.
- Aprobador y fecha de aprobación.
- Fecha de implementación y resultado.

## 6. Cambios al SGSI (6.3)

Los cambios al propio SGSI (alcance, metodología de riesgos, estructura organizacional, políticas) se planifican considerando su propósito, consecuencias, la integridad del sistema, los recursos y la reasignación de responsabilidades, y se aprueban por la Dirección General o el Comité de Seguridad.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
