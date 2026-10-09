# Política de Respaldo de la Información

| Campo | Valor |
|---|---|
| Código | POL-05 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DE TI] |
| Aprobó | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.8.13, A.5.29, A.5.30, A.8.14 |

> 💡 **Cómo adaptar:** los valores de RPO y RTO deben salir del negocio, no de TI. Pregunta a cada propietario: "¿cuántas horas de trabajo puedes perder?" y "¿cuánto tiempo puedes estar sin el sistema?". Recuerda que SaaS como Microsoft 365 o Google Workspace **no respaldan por ti** más allá de su papelera y retención básica.

## 1. Propósito

Asegurar que la información y los sistemas puedan recuperarse ante pérdida, corrupción, *ransomware* o desastre, dentro de los tiempos requeridos por el negocio.

## 2. Regla 3-2-1-1-0

Toda información crítica cumple con:
- **3** copias de los datos (producción y dos respaldos).
- **2** tipos de almacenamiento distintos.
- **1** copia fuera del sitio principal o en otra región.
- **1** copia inmutable o desconectada (*offline* o *air-gapped*).
- **0** errores en las pruebas de restauración.

## 3. Catálogo de respaldos

| Sistema o información | Criticidad | Frecuencia | Retención | RPO | RTO | Ubicación | Responsable |
|---|---|---|---|---|---|---|---|
| [ERP / Base de datos principal] | Alta | Diario completo + cada [4] h incremental | [30 días / 12 meses / 5 años] | [4 h] | [8 h] | [Ubicación] | [ROL] |
| [Microsoft 365: correo, OneDrive, SharePoint] | Alta | Diario | [1 año] | [24 h] | [24 h] | [Herramienta de respaldo SaaS] | [ROL] |
| [Repositorios de código] | Alta | Diario | [90 días] | [24 h] | [24 h] | [Ubicación] | [ROL] |
| [Servidor de archivos] | Media | Diario | [30 días] | [24 h] | [48 h] | [Ubicación] | [ROL] |
| [Configuración de red y firewall] | Media | Ante cada cambio y mensual | [12 meses] | — | [24 h] | [Ubicación] | [ROL] |

> 💡 Considera los plazos legales de conservación, por ejemplo la contabilidad y la documentación fiscal.

## 4. Requisitos de seguridad

1. Los respaldos se **cifran** en tránsito y en reposo (POL-06).
2. Las credenciales de administración de respaldos son distintas de las del dominio o directorio principal y requieren MFA.
3. Al menos una copia es **inmutable** durante el periodo de retención mínimo.
4. Los respaldos se protegen con el mismo nivel de clasificación que la información que contienen.
5. Se monitorea diariamente el resultado de los trabajos de respaldo y se atienden los fallos en un máximo de [1] día hábil.

## 5. Pruebas de restauración

| Tipo de prueba | Frecuencia | Evidencia |
|---|---|---|
| Restauración de archivos individuales | Mensual | Ticket o registro con resultado |
| Restauración completa de un sistema crítico | Semestral | Informe con tiempo real de recuperación frente al RTO |
| Ejercicio de recuperación ante *ransomware* | Anual | Informe del ejercicio y acciones de mejora |

Si la prueba excede el RTO o falla, se registra como no conformidad (PRO-05).

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
