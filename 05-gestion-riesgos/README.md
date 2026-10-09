# Gestión de riesgos

Cláusulas 6.1.2, 6.1.3, 8.2 y 8.3 de ISO/IEC 27001:2022. La metodología está en [PRO-01](../03-procedimientos/PRO-01-gestion-riesgos.md).

| Archivo | Uso |
|---|---|
| [`matriz-riesgos.xlsx`](matriz-riesgos.xlsx) | Inventario de activos, evaluación de riesgos, plan de tratamiento y mapa de calor |
| [`catalogo-amenazas.csv`](catalogo-amenazas.csv) | 30 amenazas frecuentes en PyMEs, con categoría y dimensión típica afectada |
| [`catalogo-vulnerabilidades.csv`](catalogo-vulnerabilidades.csv) | 30 vulnerabilidades frecuentes |

## Hojas de la matriz

| Hoja | Contenido |
|---|---|
| Instrucciones | Orden de llenado y código de colores |
| Inventario de activos | Activos con propietario, clasificación y valoración C, I, D; criticidad calculada |
| Evaluación de riesgos | Escenarios activo–amenaza–vulnerabilidad, nivel inherente y residual con clasificación automática, y verificación contra el apetito de riesgo |
| Plan de tratamiento | Acciones con responsable, controles del Anexo A, fechas, avance y detección de acciones vencidas |
| Mapa de calor | Matrices 5 × 5 de riesgo inherente y residual, resumen por nivel e indicadores de alerta |
| Escalas | Criterios de probabilidad e impacto, umbrales de nivel y apetito de riesgo editables |
| Catálogos | Amenazas y vulnerabilidades que alimentan las listas desplegables |

## Características

- Listas desplegables para activos, amenazas, vulnerabilidades y tratamiento.
- Nivel de riesgo = Probabilidad × Impacto, con clasificación automática Bajo / Medio / Alto / Crítico.
- Umbrales y apetito de riesgo configurables en la hoja *Escalas*.
- 200 filas preparadas con fórmulas en cada hoja de registro.
- Ejemplos realistas de una PyME de servicios (5 activos, 5 riesgos, 4 acciones) para guiar el llenado.

> 💡 Compatible con Microsoft Excel, LibreOffice Calc y Google Sheets.
