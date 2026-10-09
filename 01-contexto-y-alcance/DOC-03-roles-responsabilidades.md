# Roles y responsabilidades del SGSI

| Campo | Valor |
|---|---|
| Código | DOC-03 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | 5.1, 5.3, A.5.2, A.5.3, A.5.4 |

> 💡 **Cómo adaptar:** en organizaciones pequeñas una persona puede tener varios roles. Lo importante es que estén asignados y que se respete la segregación de funciones donde el riesgo lo exige; por ejemplo, quien administra un sistema no debería ser quien audita sus accesos.

## 1. Roles

### Dirección General
- Demostrar liderazgo y compromiso con el SGSI.
- Aprobar la política de seguridad, los objetivos y el apetito de riesgo.
- Asegurar los recursos necesarios.
- Presidir la revisión por la dirección.
- Aceptar formalmente los riesgos residuales que superen el umbral definido en PRO-01.

### Comité de Seguridad de la Información
**Integrantes:** [Dirección General], [Responsable del SGSI], [Responsable de TI], [Responsable de RR. HH.], [Responsable de Operaciones].
**Frecuencia:** [trimestral] y de forma extraordinaria ante incidentes graves.
- Dar seguimiento al plan de tratamiento de riesgos y a los objetivos.
- Revisar incidentes relevantes y resultados de auditorías.
- Priorizar iniciativas de seguridad.

### Responsable del SGSI
**Asignado a:** [NOMBRE Y PUESTO]
- Coordinar la implementación, operación y mejora del SGSI.
- Mantener la metodología de riesgos, la SoA y la información documentada.
- Informar a la dirección sobre el desempeño del SGSI.
- Coordinar auditorías internas y externas.
- Ser el punto de contacto con autoridades y grupos de interés especial (A.5.5, A.5.6).

### Responsable de Tecnologías de la Información
**Asignado a:** [NOMBRE Y PUESTO]
- Implementar y operar los controles técnicos.
- Gestionar accesos, respaldos, vulnerabilidades y cambios.
- Liderar técnicamente la respuesta a incidentes.

### Propietarios de activos
- Clasificar la información de sus activos.
- Autorizar y revisar los accesos.
- Asegurar que el activo se protege de acuerdo con su clasificación.

### Propietarios de riesgos
- Decidir el tratamiento de los riesgos asignados.
- Dar seguimiento a la ejecución de los controles y aceptar el riesgo residual dentro de su nivel de autoridad.

### Recursos Humanos
- Verificar antecedentes en la contratación según la legislación aplicable (A.6.1).
- Incluir responsabilidades de seguridad en contratos (A.6.2).
- Notificar altas, cambios y bajas a TI de forma oportuna (A.6.5).
- Coordinar el proceso disciplinario (A.6.4).

### Colaboradores
- Cumplir las políticas del SGSI.
- Reportar eventos y debilidades de seguridad (A.6.8).
- Participar en la concientización.

### Auditor interno
- Auditar el SGSI con objetividad e imparcialidad, sin auditar su propio trabajo.

## 2. Matriz RACI de procesos clave

R = Responsable · A = Aprueba · C = Consultado · I = Informado

| Proceso | Dirección | Resp. SGSI | TI | RR. HH. | Propietario de activo |
|---|---|---|---|---|---|
| Política de seguridad | A | R | C | C | I |
| Evaluación de riesgos | I | R | C | C | C |
| Aceptación de riesgo residual | A | C | C | — | R |
| Declaración de Aplicabilidad | A | R | C | I | I |
| Gestión de accesos | — | I | R | C | A |
| Gestión de incidentes | I | A | R | C | C |
| Auditoría interna | I | A | C | C | C |
| Revisión por la dirección | A/R | R | C | C | I |

## 3. Segregación de funciones

| Actividad | No debe ser realizada por la misma persona que |
|---|---|
| Aprobación de accesos | Solicita el acceso |
| Paso de cambios a producción | Desarrolló el cambio, salvo excepción documentada |
| Revisión de bitácoras de administradores | Es el administrador revisado |
| Auditoría interna de un proceso | Opera ese proceso |

Cuando el tamaño de la organización impida la segregación, se aplicarán controles compensatorios como revisión posterior por un tercero o registro inalterable de actividades.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
