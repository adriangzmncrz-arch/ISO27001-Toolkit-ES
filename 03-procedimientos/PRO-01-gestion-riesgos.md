# Procedimiento de Gestión de Riesgos de Seguridad de la Información

| Campo | Valor |
|---|---|
| Código | PRO-01 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | 6.1.1, 6.1.2, 6.1.3, 8.2, 8.3; ISO/IEC 27005:2022 como guía |

> 💡 **Cómo adaptar:** la norma exige que la evaluación produzca **resultados coherentes, válidos y comparables** cuando se repite. Por eso las escalas de este documento deben coincidir exactamente con las de la [matriz de riesgos](../05-gestion-riesgos/). Si cambias una, cambia la otra.

## 1. Propósito

Establecer la metodología para identificar, analizar, evaluar y tratar los riesgos de seguridad de la información dentro del alcance del SGSI.

## 2. Frecuencia

- **Evaluación completa:** al menos una vez al año.
- **Evaluación puntual:** ante cambios significativos (nuevo sistema, proveedor crítico, proceso, sede), incidentes graves o hallazgos de auditoría relevantes.

## 3. Enfoque

Se utiliza un enfoque **basado en activos y escenarios**: para cada activo o grupo de activos se identifican escenarios de riesgo compuestos por una amenaza que explota una vulnerabilidad y afecta la confidencialidad, integridad o disponibilidad.

## 4. Etapas

### 4.1 Identificación de activos
Se registran en la hoja *Inventario de activos* con su propietario, clasificación y valoración de C, I y D.

### 4.2 Identificación de riesgos
Para cada activo se identifican amenazas y vulnerabilidades, apoyándose en los catálogos de la matriz. Cada riesgo se describe con la estructura:

> **Por** [amenaza] **que aprovecha** [vulnerabilidad], **podría** [consecuencia] **afectando** [dimensión C/I/D] **de** [activo].

Cada riesgo tiene un **propietario del riesgo** asignado.

### 4.3 Análisis

**Escala de probabilidad**

| Valor | Nivel | Criterio |
|---|---|---|
| 1 | Muy baja | Puede ocurrir solo en circunstancias excepcionales; no ha ocurrido en la organización ni en el sector cercano |
| 2 | Baja | Podría ocurrir alguna vez en los próximos 5 años |
| 3 | Media | Podría ocurrir alguna vez en los próximos 2 años, o ya ha ocurrido en organizaciones similares |
| 4 | Alta | Es probable que ocurra en el próximo año, o ha ocurrido en la organización |
| 5 | Muy alta | Ocurre o se espera que ocurra varias veces al año |

**Escala de impacto** (se toma el valor más alto entre los criterios)

| Valor | Nivel | Financiero | Operativo | Legal / contractual | Reputacional |
|---|---|---|---|---|---|
| 1 | Muy bajo | < [$50,000] MXN | Interrupción menor a 1 h sin efecto en clientes | Ninguno | Sin trascendencia externa |
| 2 | Bajo | [$50,000 – $250,000] | Interrupción de hasta 4 h | Incumplimiento menor subsanable | Queja aislada de un cliente |
| 3 | Medio | [$250,000 – $1,000,000] | Interrupción de hasta 1 día de un servicio | Penalización contractual | Varios clientes afectados |
| 4 | Alto | [$1,000,000 – $5,000,000] | Interrupción de 1 a 3 días de servicios críticos | Sanción de autoridad o demanda | Cobertura en medios locales; pérdida de clientes |
| 5 | Muy alto | > [$5,000,000] | Interrupción de más de 3 días o pérdida irrecuperable de información | Sanción grave, suspensión de operaciones | Daño reputacional nacional o pérdida de clientes clave |

> 💡 Ajusta los montos al tamaño de tu organización. Una referencia útil: el nivel 5 debería ser un impacto que ponga en riesgo la viabilidad del negocio.

**Nivel de riesgo** = Probabilidad × Impacto (valores de 1 a 25)

|  | **Impacto 1** | **2** | **3** | **4** | **5** |
|---|---|---|---|---|---|
| **Probabilidad 5** | 5 🟡 | 10 🟠 | 15 🔴 | 20 🔴 | 25 🔴 |
| **4** | 4 🟢 | 8 🟡 | 12 🟠 | 16 🔴 | 20 🔴 |
| **3** | 3 🟢 | 6 🟡 | 9 🟠 | 12 🟠 | 15 🔴 |
| **2** | 2 🟢 | 4 🟢 | 6 🟡 | 8 🟡 | 10 🟠 |
| **1** | 1 🟢 | 2 🟢 | 3 🟢 | 4 🟢 | 5 🟡 |

### 4.4 Evaluación y criterios de aceptación

| Nivel | Rango | Decisión | Quién puede aceptar el riesgo residual |
|---|---|---|---|
| 🟢 **Bajo** | 1 – 4 | Aceptable. Se monitorea. | Propietario del riesgo |
| 🟡 **Medio** | 5 – 8 | Tratar si el costo es razonable; de lo contrario, aceptar con justificación. | Propietario del riesgo y Responsable del SGSI |
| 🟠 **Alto** | 9 – 14 | Debe tratarse. Plan de tratamiento en un máximo de [90] días. | Dirección General |
| 🔴 **Crítico** | 15 – 25 | Tratamiento inmediato. Plan en un máximo de [30] días; medidas de contención urgentes. | Dirección General, de forma excepcional y por escrito |

**Apetito de riesgo:** la organización acepta riesgos residuales de nivel **Bajo** y **Medio**. Los riesgos residuales **Alto** o **Crítico** solo se aceptan de forma temporal, con aprobación de la Dirección General y fecha de revisión.

### 4.5 Tratamiento

| Opción | Descripción |
|---|---|
| **Mitigar** | Aplicar controles que reduzcan la probabilidad o el impacto. |
| **Transferir** | Compartir el riesgo con un tercero: seguro, contrato con cláusulas de responsabilidad. La responsabilidad sobre la información no se transfiere. |
| **Evitar** | Eliminar la actividad o el activo que genera el riesgo. |
| **Aceptar** | Asumir el riesgo de forma informada, dentro de los criterios de aceptación. |

Para cada riesgo tratado se determinan los controles necesarios, se **comparan con los 93 controles del Anexo A** para verificar que no se omite ninguno necesario y se registran en el plan de tratamiento con responsable, fecha y recursos. Los resultados alimentan la Declaración de Aplicabilidad.

### 4.6 Riesgo residual y aprobación

Tras definir el tratamiento se estima el riesgo residual con las mismas escalas. El plan de tratamiento y los riesgos residuales son aprobados por los propietarios de los riesgos según la tabla 4.4.

## 5. Seguimiento

- El Comité de Seguridad revisa el avance del plan de tratamiento [trimestralmente].
- Los resultados se presentan en la revisión por la dirección (PRO-08).

## 6. Registros

| Registro | Ubicación | Retención |
|---|---|---|
| Inventario de activos | Matriz de riesgos | Vigente + 3 años |
| Evaluación de riesgos | Matriz de riesgos | 3 años |
| Plan de tratamiento | Matriz de riesgos | 3 años |
| Aprobaciones de riesgo residual | [Correo / acta / flujo de aprobación] | 3 años |

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
