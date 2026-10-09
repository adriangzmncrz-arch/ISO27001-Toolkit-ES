# Guía de uso

Esta guía te ayuda a convertir las plantillas en un SGSI propio. El orden importa: las decisiones de las primeras fases determinan qué documentos necesitas después.

## Antes de empezar

- **Consigue la norma.** Las plantillas no sustituyen la lectura de ISO/IEC 27001:2022. ISO/IEC 27002:2022 es muy recomendable porque explica cómo implementar cada control.
- **Obtén el compromiso de la dirección.** Sin un patrocinador con autoridad, el SGSI se queda en papel.
- **Define quién es el Responsable del SGSI.** Será el propietario de la mayoría de los documentos.

## Ruta de implementación

### Fase 1 — Contexto y alcance (semanas 1 a 3)

| Paso | Plantilla | Resultado |
|---|---|---|
| 1 | [DOC-01 Contexto de la organización](../01-contexto-y-alcance/DOC-01-contexto-organizacion.md) | Cuestiones internas y externas, partes interesadas y requisitos legales |
| 2 | [DOC-02 Alcance del SGSI](../01-contexto-y-alcance/DOC-02-alcance-sgsi.md) | Límites del sistema: procesos, sedes, tecnología, exclusiones |
| 3 | [DOC-03 Roles y responsabilidades](../01-contexto-y-alcance/DOC-03-roles-responsabilidades.md) | Quién hace qué en el SGSI |
| 4 | [POL-00 Política de seguridad](../02-politicas/POL-00-politica-seguridad-informacion.md) | Compromiso de la dirección, aprobado y comunicado |

### Fase 2 — Riesgos (semanas 3 a 7)

| Paso | Plantilla | Resultado |
|---|---|---|
| 5 | [PRO-01 Gestión de riesgos](../03-procedimientos/PRO-01-gestion-riesgos.md) | Metodología: escalas, criterios de aceptación |
| 6 | [Matriz de riesgos](../05-gestion-riesgos/) — hoja *Inventario de activos* | Activos de información dentro del alcance |
| 7 | Matriz de riesgos — hoja *Evaluación de riesgos* | Riesgos identificados, analizados y evaluados |
| 8 | Matriz de riesgos — hoja *Plan de tratamiento* | Controles, responsables, fechas y riesgo residual |

### Fase 3 — Declaración de Aplicabilidad (semanas 7 a 8)

| Paso | Plantilla | Resultado |
|---|---|---|
| 9 | [SoA](../04-declaracion-aplicabilidad/) | Los 93 controles del Anexo A con su justificación de inclusión o exclusión y su estado |

> La SoA se deriva del tratamiento de riesgos, no al revés. Un control se incluye porque trata un riesgo, porque lo exige un requisito legal o contractual, o porque la organización decide adoptarlo como buena práctica.

### Fase 4 — Políticas y procedimientos (semanas 8 a 14)

Adapta únicamente las políticas y procedimientos que respaldan controles aplicables en tu SoA. Revisa el [mapa documental](mapa-documental.md) para ver qué cubre cada uno.

### Fase 5 — Operación y evidencia (meses 4 a 6)

- Ejecuta los controles y **genera registros** con los formatos de [`06-registros/`](../06-registros/).
- Lleva a cabo la concientización y registra la asistencia ([REG-07](../06-registros/REG-07-competencias-concientizacion.md)).
- Mide tus objetivos ([REG-01](../06-registros/REG-01-objetivos-sgsi.md)).

### Fase 6 — Verificación y mejora (meses 6 a 8)

- Auditoría interna completa ([PRO-04](../03-procedimientos/PRO-04-auditoria-interna.md)).
- Revisión por la dirección ([PRO-08](../03-procedimientos/PRO-08-revision-direccion.md)).
- Atención de no conformidades ([PRO-05](../03-procedimientos/PRO-05-no-conformidades-acciones-correctivas.md)).

Para una auditoría de certificación, los organismos certificadores suelen esperar que el SGSI haya operado algunos meses con evidencia de auditoría interna y revisión por la dirección completas.

## Cómo personalizar las plantillas

1. **Busca y reemplaza los marcadores.** Todo lo que está entre corchetes `[ ]` debe sustituirse.
2. **Elimina los bloques de orientación.** Los párrafos que comienzan con `> 💡 Cómo adaptar` son instrucciones para ti; bórralos de la versión final.
3. **Ajusta la exigencia a tu realidad.** Si una política dice "trimestral" y tu equipo solo puede hacerlo semestralmente, escribe semestral y trata el riesgo residual. Un auditor encuentra más grave incumplir lo que escribiste que haber elegido un plazo más largo.
4. **Mantén la trazabilidad.** No elimines las referencias a cláusulas y controles; facilitan la auditoría.
5. **Convierte al formato que uses.** Los Markdown se convierten fácilmente a Word o PDF, por ejemplo con [Pandoc](https://pandoc.org/): `pandoc POL-00-politica-seguridad-informacion.md -o POL-00.docx`.

## Errores comunes que estas plantillas buscan evitar

- Copiar políticas genéricas que nadie en la organización conoce ni cumple.
- Hacer la SoA antes del análisis de riesgos.
- Excluir controles sin una justificación vinculada al alcance o a los riesgos.
- No conservar evidencia de la operación: "lo hacemos pero no queda registro".
- Tratar el SGSI como un proyecto de TI en vez de un sistema de gestión de la organización.
