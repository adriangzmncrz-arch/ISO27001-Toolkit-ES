# Política de Seguridad en la Relación con Proveedores

| Campo | Valor |
|---|---|
| Código | POL-04 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.5.19, A.5.20, A.5.21, A.5.22, A.5.23 |

> 💡 **Cómo adaptar:** no todos los proveedores requieren el mismo nivel de revisión. La clasificación por criticidad evita evaluar a la papelería con el mismo rigor que a tu proveedor de nube. Para proveedores grandes (AWS, Microsoft, Google) no vas a negociar el contrato: revisa sus certificaciones e informes y configura bien tu parte del modelo de responsabilidad compartida.

## 1. Propósito

Mantener un nivel adecuado de seguridad de la información en los servicios y productos que proporcionan los proveedores.

## 2. Clasificación de proveedores

| Criticidad | Criterio | Ejemplos |
|---|---|---|
| **Alta** | Accede, procesa o almacena información Confidencial o Restringida, o su falla interrumpe un servicio crítico | Nube, hospedaje, desarrollo externo, nómina, soporte de TI con acceso administrativo |
| **Media** | Acceso limitado a información de Uso interno o a instalaciones | Mantenimiento de equipos, servicios de limpieza con acceso a oficinas |
| **Baja** | Sin acceso a información ni sistemas | Papelería, cafetería |

## 3. Ciclo de vida del proveedor

### 3.1 Selección y evaluación
| Criticidad | Requisitos previos a la contratación |
|---|---|
| Alta | Cuestionario de seguridad; revisión de certificaciones (ISO/IEC 27001, SOC 2 tipo II) o evidencia equivalente; evaluación de riesgos documentada |
| Media | Cuestionario simplificado; acuerdo de confidencialidad |
| Baja | Ninguno adicional |

### 3.2 Requisitos contractuales (A.5.20)
Los contratos con proveedores de criticidad Alta incluyen, según aplique:
- Confidencialidad y uso de la información únicamente para el servicio contratado.
- Cumplimiento de la legislación de protección de datos personales y, cuando corresponda, la figura de encargado.
- Notificación de incidentes de seguridad en un plazo máximo de **[24 / 48] horas**.
- Derecho de auditoría o entrega de informes de auditoría independientes.
- Controles mínimos de seguridad: MFA, cifrado, respaldos, gestión de vulnerabilidades.
- Restricciones a la subcontratación y obligación de trasladar los requisitos a los subcontratistas.
- Devolución y eliminación segura de la información al terminar el contrato.
- Niveles de servicio y continuidad.

### 3.3 Seguimiento (A.5.22)
| Criticidad | Revisión |
|---|---|
| Alta | Anual: revisión de certificaciones vigentes, incidentes, desempeño del SLA y cambios en el servicio |
| Media | Cada dos años o ante cambios |
| Baja | No requerida |

### 3.4 Terminación
- Revocar todos los accesos del proveedor.
- Recuperar la información y obtener constancia de su eliminación.
- Recuperar activos entregados.

## 4. Servicios en la nube (A.5.23)

Además de lo anterior, para servicios en la nube se debe:
- Identificar la región donde se almacenan los datos y validar que cumple los requisitos legales y contractuales.
- Documentar el modelo de responsabilidad compartida y los controles a cargo de la organización.
- Habilitar MFA, registros de auditoría y alertas de seguridad disponibles.
- Definir cómo se recuperará la información si se termina el servicio (estrategia de salida).

## 5. Registro de proveedores

El Responsable del SGSI mantiene un registro con, al menos: proveedor, servicio, criticidad, información a la que accede, fecha de evaluación, certificaciones, vigencia del contrato y responsable interno.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
