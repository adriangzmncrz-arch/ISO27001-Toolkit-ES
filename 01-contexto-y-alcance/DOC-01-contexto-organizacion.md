# Contexto de la organización y partes interesadas

| Campo | Valor |
|---|---|
| Código | DOC-01 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | 4.1, 4.2, A.5.31 |

> 💡 **Cómo adaptar:** este documento se construye en un taller de 2 a 3 horas con la dirección y los responsables de área. Las tablas incluyen ejemplos típicos de una PyME de servicios; sustitúyelos por los tuyos. Revísalo al menos una vez al año y cada vez que cambie algo relevante en el negocio.

## 1. Propósito

Identificar las cuestiones internas y externas que afectan la capacidad de [NOMBRE DE LA ORGANIZACIÓN] para lograr los resultados previstos de su SGSI, así como las partes interesadas y sus requisitos.

## 2. Descripción de la organización

| Aspecto | Descripción |
|---|---|
| Actividad principal | [Ejemplo: servicios de consultoría y desarrollo de software] |
| Número de colaboradores | [Ejemplo: 45] |
| Sedes | [Ejemplo: oficina central en Guadalajara, Jal.; trabajo híbrido] |
| Principales clientes | [Ejemplo: sector financiero y manufactura] |
| Infraestructura tecnológica | [Ejemplo: Microsoft 365, AWS, ERP en la nube] |
| Resultados previstos del SGSI | [Ejemplo: proteger la información de clientes, cumplir requisitos contractuales, obtener la certificación ISO/IEC 27001] |

## 3. Cuestiones internas y externas

> 💡 Una técnica útil es el análisis PESTEL para lo externo y el análisis de capacidades (personas, procesos, tecnología) para lo interno. Lo importante es que cada cuestión sea concreta y tenga un efecto sobre el SGSI.

### 3.1 Cuestiones externas

| ID | Categoría | Cuestión | Efecto en el SGSI |
|---|---|---|---|
| CE-01 | Legal | Entrada en vigor de la nueva LFPDPPP (marzo de 2025) | Revisar avisos de privacidad y medidas de seguridad para datos personales |
| CE-02 | Mercado | Clientes que exigen certificación o cuestionarios de seguridad a sus proveedores | Necesidad de evidencia formal de controles |
| CE-03 | Tecnológica | Aumento de ataques de *phishing* y *ransomware* dirigidos a PyMEs | Priorizar concientización, respaldos y MFA |
| CE-04 | Tecnológica | Dependencia de proveedores de servicios en la nube | Gestión de proveedores y continuidad |
| CE-05 | [Categoría] | [Cuestión] | [Efecto] |

### 3.2 Cuestiones internas

| ID | Categoría | Cuestión | Efecto en el SGSI |
|---|---|---|---|
| CI-01 | Personas | Equipo de TI reducido, con alta carga operativa | Automatizar controles y priorizar por riesgo |
| CI-02 | Procesos | Altas y bajas de personal sin un flujo formal | Riesgo de accesos no revocados |
| CI-03 | Cultura | Trabajo híbrido consolidado | Controles para trabajo remoto y dispositivos |
| CI-04 | Estrategia | Plan de crecimiento a nuevos mercados | El SGSI debe escalar con el negocio |
| CI-05 | [Categoría] | [Cuestión] | [Efecto] |

## 4. Partes interesadas y sus requisitos

| Parte interesada | Necesidades y expectativas | Requisito que atiende el SGSI | Mecanismo |
|---|---|---|---|
| Clientes | Confidencialidad de su información; disponibilidad del servicio | Sí | Contratos, acuerdos de confidencialidad, SLA |
| Colaboradores | Protección de sus datos personales; reglas claras | Sí | POL-02, POL-10, concientización |
| Dirección / accionistas | Continuidad del negocio, reputación, cumplimiento | Sí | Revisión por la dirección |
| Proveedores críticos | Requisitos claros de seguridad | Sí | POL-04, cláusulas contractuales |
| Autoridad de protección de datos | Cumplimiento de la LFPDPPP | Sí | POL-10, avisos de privacidad |
| Aseguradora (ciberseguro) | Controles mínimos como MFA y respaldos | [Sí/No] | [Mecanismo] |
| [Parte interesada] | [Necesidad] | [Sí/No] | [Mecanismo] |

## 5. Requisitos legales, regulatorios y contractuales

> 💡 Este registro atiende el control A.5.31. Valida su contenido con tu asesor legal; la lista es orientativa para México.

| Requisito | Tipo | Aplica a | Responsable de seguimiento | Última revisión |
|---|---|---|---|---|
| Ley Federal de Protección de Datos Personales en Posesión de los Particulares (2025) y su reglamento | Legal | Datos personales de clientes, colaboradores y prospectos | [ROL] | [AAAA-MM-DD] |
| Ley Federal del Derecho de Autor (software y licencias) | Legal | Uso de software | [ROL] | [AAAA-MM-DD] |
| Código de Comercio — conservación de mensajes de datos | Legal | Registros electrónicos comerciales | [ROL] | [AAAA-MM-DD] |
| Disposiciones fiscales (CFDI y conservación de contabilidad) | Legal | Información contable y fiscal | [ROL] | [AAAA-MM-DD] |
| Ley Federal del Trabajo (expedientes de personal) | Legal | Información de colaboradores | [ROL] | [AAAA-MM-DD] |
| Contrato con [CLIENTE] — cláusula de confidencialidad y notificación de incidentes | Contractual | [Servicio] | [ROL] | [AAAA-MM-DD] |
| [Normativa sectorial, por ejemplo, disposiciones de la CNBV si das servicio al sector financiero] | Regulatorio | [Alcance] | [ROL] | [AAAA-MM-DD] |

## 6. Revisión

Este documento se revisa al menos una vez al año, en la revisión por la dirección, y cada vez que ocurra un cambio significativo: nueva línea de negocio, fusión, cambio regulatorio, cambio tecnológico mayor o incidente grave.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
