# Política de Clasificación de la Información

| Campo | Valor |
|---|---|
| Código | POL-03 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.5.12, A.5.13, A.5.14, A.7.10, A.7.14, A.8.10, A.8.12 |

> 💡 **Cómo adaptar:** cuatro niveles son suficientes para la mayoría de las organizaciones. Más niveles generan confusión y la gente termina clasificando todo igual. Si usas Microsoft Purview u otra herramienta de etiquetado, alinea los nombres de las etiquetas con esta tabla.

## 1. Propósito

Asegurar que la información reciba un nivel de protección acorde con su importancia para la organización y con los requisitos legales y contractuales.

## 2. Niveles de clasificación

| Nivel | Definición | Ejemplos |
|---|---|---|
| **Público** | Información aprobada para divulgación externa. Su divulgación no causa daño. | Sitio web, folletos, ofertas de empleo publicadas |
| **Uso interno** | Información de operación ordinaria. Su divulgación causaría un daño menor. | Políticas internas, directorio, procedimientos operativos |
| **Confidencial** | Información sensible para el negocio o los clientes. Su divulgación causaría un daño significativo. | Información de clientes, propuestas comerciales, contratos, datos personales |
| **Restringida** | Información crítica. Su divulgación causaría un daño grave, sanciones o pérdida de confianza. | Credenciales, llaves criptográficas, datos personales sensibles, estrategia de fusiones, información financiera no publicada |

> Información sin etiqueta se trata como **Uso interno**. En caso de duda, se aplica el nivel más alto.

## 3. Responsabilidades

- El **propietario del activo** clasifica la información y revisa la clasificación al menos una vez al año.
- Los **usuarios** respetan las reglas de manejo según el nivel.
- La información recibida de terceros se protege según lo acordado contractualmente o, en su defecto, como Confidencial.

## 4. Etiquetado (A.5.13)

| Medio | Cómo se etiqueta |
|---|---|
| Documentos electrónicos | Encabezado o pie de página con el nivel; etiqueta de sensibilidad si la plataforma lo permite |
| Correo electrónico | Etiqueta de sensibilidad o prefijo en el asunto: `[CONFIDENCIAL]` |
| Documentos impresos | Nivel visible en la portada y en cada página |
| Medios removibles | Etiqueta física con el nivel |
| Sistemas y bases de datos | Registrado en el inventario de activos |

La información Pública y de Uso interno no requiere etiqueta obligatoria.

## 5. Reglas de manejo

| Actividad | Uso interno | Confidencial | Restringida |
|---|---|---|---|
| Acceso | Personal de la organización | Según necesidad de conocer, autorizado por el propietario | Personas nominadas por el propietario; lista revisada trimestralmente |
| Almacenamiento | Repositorios corporativos | Repositorios corporativos con control de acceso | Repositorios con control de acceso y cifrado; bóveda para credenciales |
| Envío por correo interno | Permitido | Permitido | Solo cifrado o mediante enlace con acceso restringido |
| Envío externo | Con autorización del área | Cifrado o enlace seguro con expiración; acuerdo de confidencialidad vigente | Prohibido salvo autorización expresa del propietario y cifrado |
| Impresión | Permitida | Solo cuando sea necesario; recoger de inmediato | Evitar; impresión segura con liberación por credencial |
| Medios removibles | Permitidos si están autorizados | Solo cifrados | Prohibidos salvo autorización y cifrado |
| Herramientas de IA | Herramientas aprobadas | Solo con contrato empresarial | Prohibido |
| Eliminación | Borrado normal | Borrado seguro; trituración del papel | Borrado seguro certificado; trituración de corte cruzado |

## 6. Eliminación de información y equipos (A.7.14, A.8.10)

- Los equipos que se dan de baja, reasignan o envían a reparación externa se someten a borrado seguro o destrucción del almacenamiento.
- Se conserva constancia de la destrucción (certificado del proveedor o registro interno) para equipos que contuvieron información Confidencial o Restringida.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
