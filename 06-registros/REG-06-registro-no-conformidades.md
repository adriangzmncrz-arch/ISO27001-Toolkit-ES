# Registro de No Conformidades, Acciones Correctivas y Mejoras

| Campo | Valor |
|---|---|
| Código | REG-06 |
| Propietario | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | 10.1, 10.2 |

> 💡 **Cómo adaptar:** este registro funciona mejor como hoja de cálculo o lista en tu herramienta de tickets o en SharePoint. La tabla de abajo define las columnas. Conserva cada registro aunque se cierre: es la evidencia del ciclo de mejora.

## Columnas del registro

| Columna | Descripción |
|---|---|
| ID | NC-[AAAA]-[nnn] para no conformidades; OM-[AAAA]-[nnn] para mejoras |
| Fecha de detección | |
| Fuente | Auditoría interna, auditoría externa, incidente, indicador, revisión por la dirección, queja, otro |
| Tipo | NC mayor, NC menor, observación, oportunidad de mejora |
| Requisito | Cláusula, control o documento interno |
| Descripción | Qué ocurrió, con evidencia |
| Corrección inmediata | Qué se hizo para controlar el efecto |
| Causa raíz | Resultado del análisis (5 porqués, Ishikawa) |
| ¿Puede ocurrir en otro lugar? | Sí/No y dónde |
| Acción correctiva | Qué se cambia para eliminar la causa |
| Responsable | |
| Fecha compromiso | |
| Fecha de implementación | |
| Verificación de eficacia | Cómo se verificó, cuándo y por quién |
| Resultado | Eficaz / no eficaz (reabrir) |
| Estado | Abierta, en curso, en verificación, cerrada |

## Ejemplo

| ID | Fecha | Fuente | Tipo | Requisito | Descripción | Corrección | Causa raíz | Acción correctiva | Responsable | Compromiso | Verificación | Estado |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| NC-2026-001 | 2026-03-12 | Auditoría interna AI-03 | NC menor | A.5.18; PRO-07 §4 | 2 de 6 bajas revisadas conservaban acceso al CRM más de 10 días | Se deshabilitaron ambas cuentas el 12/03 | El CRM no está integrado al SSO y la baja depende de un paso manual sin control | Integrar el CRM al SSO; mientras tanto, agregar casilla obligatoria "CRM" en el ticket de baja | [Resp. TI] | 2026-05-30 | 2026-07-15: revisión de 8 bajas posteriores, todas conformes | Cerrada |
