# Política de Gestión de Vulnerabilidades Técnicas

| Campo | Valor |
|---|---|
| Código | POL-09 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DE TI] |
| Aprobó | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.5.7, A.8.7, A.8.8, A.8.9, A.8.19 |

> 💡 **Cómo adaptar:** los plazos de remediación de la sección 4 son un punto de partida razonable. Mídelos: un indicador de "porcentaje de vulnerabilidades críticas atendidas en plazo" es de los más útiles para la revisión por la dirección.

## 1. Propósito

Identificar, evaluar y corregir oportunamente las vulnerabilidades técnicas de los sistemas de la organización.

## 2. Fuentes de identificación

- Escaneos automatizados de vulnerabilidades: [HERRAMIENTA].
- Avisos de fabricantes y boletines de seguridad.
- Catálogo de vulnerabilidades explotadas activamente (por ejemplo, el catálogo KEV de CISA).
- Inteligencia de amenazas y alertas de CERT-MX (A.5.7).
- Pruebas de penetración y análisis de código (POL-07).
- Reportes de colaboradores, clientes o investigadores.

## 3. Frecuencia de escaneo

| Activo | Frecuencia |
|---|---|
| Sistemas expuestos a internet | [Semanal / continuo] |
| Servidores y servicios internos | Mensual |
| Equipos de usuario | Continuo mediante agente de EDR o gestión de parches |
| Prueba de penetración externa | Anual y ante cambios mayores |

## 4. Priorización y plazos de remediación

La severidad parte de la puntuación CVSS y se ajusta según la exposición del activo y si existe explotación activa conocida.

| Severidad | Criterio | Plazo máximo |
|---|---|---|
| **Crítica** | CVSS 9.0 – 10.0, o cualquier vulnerabilidad con explotación activa en sistemas expuestos | [7] días naturales |
| **Alta** | CVSS 7.0 – 8.9 | [30] días naturales |
| **Media** | CVSS 4.0 – 6.9 | [90] días naturales |
| **Baja** | CVSS 0.1 – 3.9 | Siguiente ciclo de mantenimiento |

## 5. Gestión de parches

1. Los parches de seguridad de sistemas operativos y aplicaciones de usuario se despliegan de forma automática tras un periodo de prueba de [3-7] días en un grupo piloto.
2. Los parches de servidores siguen el procedimiento de cambios (PRO-06); los parches críticos pueden tramitarse como cambio de emergencia.
3. El software y los sistemas sin soporte del fabricante se reemplazan o se aíslan con controles compensatorios aprobados por el Responsable del SGSI.

## 6. Excepciones

Cuando no sea posible corregir dentro del plazo, el propietario del activo documenta la justificación, los controles compensatorios y la nueva fecha. Las excepciones a vulnerabilidades críticas requieren aprobación del Responsable del SGSI y se revisan cada [30] días.

## 7. Configuración segura (A.8.9)

Los sistemas se instalan a partir de configuraciones base endurecidas (por ejemplo, CIS Benchmarks), con servicios innecesarios deshabilitados y credenciales predeterminadas cambiadas.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
