# Procedimiento de Control de la Información Documentada

| Campo | Valor |
|---|---|
| Código | PRO-03 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | 7.5.1, 7.5.2, 7.5.3, A.5.33 |

> 💡 **Cómo adaptar:** si ya tienes un sistema de gestión ISO 9001, probablemente ya tienes este procedimiento: intégralos en uno solo. Si usas SharePoint o Google Drive, aprovecha el historial de versiones y los flujos de aprobación nativos en lugar de llevar todo a mano.

## 1. Propósito

Asegurar que la información documentada del SGSI esté identificada, aprobada, disponible donde se necesita, protegida y actualizada.

## 2. Tipos de información documentada

| Tipo | Características | Ejemplos |
|---|---|---|
| **Documento** | Describe cómo se hacen las cosas. Se actualiza y versiona. | Políticas, procedimientos, instructivos |
| **Registro** | Evidencia de lo que se hizo. No se modifica después de creado. | Actas, informes de auditoría, bitácoras, reportes de incidentes |

## 3. Identificación

Cada documento incluye en su encabezado: código, título, versión, fecha de emisión, propietario, quién aprobó y clasificación. Los códigos siguen la estructura:

| Prefijo | Tipo |
|---|---|
| DOC-nn | Documentos de contexto |
| POL-nn | Políticas |
| PRO-nn | Procedimientos |
| INS-nn | Instructivos |
| REG-nn | Formatos de registro |

## 4. Elaboración, revisión y aprobación

| Paso | Responsable |
|---|---|
| 1. Elaborar o modificar el borrador | Propietario del documento |
| 2. Revisar contenido técnico y coherencia con el SGSI | Responsable del SGSI |
| 3. Aprobar | Según la tabla siguiente |
| 4. Publicar y comunicar | Responsable del SGSI |

| Tipo de documento | Aprueba |
|---|---|
| POL-00, DOC-01, DOC-02, PRO-01 | Dirección General |
| Políticas temáticas | Responsable del SGSI o Dirección General |
| Procedimientos e instructivos | Responsable del SGSI |

**Versionado:** versión mayor (1.0 → 2.0) para cambios de fondo; versión menor (1.0 → 1.1) para correcciones de forma. Los borradores usan 0.x.

## 5. Distribución y acceso

- La versión vigente se publica en [REPOSITORIO OFICIAL, por ejemplo: sitio de SharePoint "SGSI"].
- Las copias impresas o descargadas son **copias no controladas**; la versión válida es la del repositorio oficial.
- El acceso al repositorio se otorga según la clasificación del documento.

## 6. Revisión periódica

Cada documento se revisa al menos **una vez al año** o cuando cambien las condiciones que lo afectan. Si no requiere cambios, se registra la revisión en el control de cambios.

## 7. Documentos obsoletos

Los documentos obsoletos se retiran del repositorio oficial y se conservan en un área de archivo, identificados como "OBSOLETO", durante [3] años.

## 8. Conservación de registros

| Registro | Retención mínima |
|---|---|
| Registros del SGSI (auditorías, revisiones, no conformidades, riesgos) | [3] años o un ciclo de certificación |
| Reportes de incidentes | [5] años |
| Bitácoras de sistemas | [12] meses en línea; según requisitos legales o contractuales |
| Evidencia de capacitación | Duración de la relación laboral + [2] años |

Los registros se protegen contra modificación, pérdida y acceso no autorizado. Su eliminación al término del periodo se realiza de forma segura (POL-03).

## 9. Documentos de origen externo

Las normas, contratos, leyes y documentos de proveedores relevantes para el SGSI se registran en una lista de documentos externos, con su versión vigente y el responsable de dar seguimiento a sus actualizaciones.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
