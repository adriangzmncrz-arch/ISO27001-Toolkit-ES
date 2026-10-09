# Alcance del Sistema de Gestión de Seguridad de la Información

| Campo | Valor |
|---|---|
| Código | DOC-02 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Público |
| Referencias ISO/IEC 27001:2022 | 4.3, 4.4 |

> 💡 **Cómo adaptar:** el alcance aparece en tu certificado, así que debe ser preciso. Un alcance demasiado amplio vuelve costosa la implementación; uno demasiado estrecho no convence a tus clientes. Empieza por los procesos que tus clientes valoran y amplía después.

## 1. Declaración de alcance

> El Sistema de Gestión de Seguridad de la Información de **[NOMBRE DE LA ORGANIZACIÓN]** aplica a **[PROCESOS O SERVICIOS, por ejemplo: la prestación de servicios de consultoría en ciberseguridad y el desarrollo de software a la medida]**, llevados a cabo desde **[SEDES, por ejemplo: sus oficinas en Zapopan, Jalisco, y en modalidad de trabajo remoto]**, de acuerdo con la Declaración de Aplicabilidad versión **[X.X]** de fecha **[AAAA-MM-DD]**.

## 2. Elementos incluidos

### 2.1 Procesos y servicios
- [Proceso 1: por ejemplo, comercialización y contratación de servicios]
- [Proceso 2: por ejemplo, prestación del servicio]
- [Proceso 3: por ejemplo, soporte técnico al cliente]
- Procesos de apoyo: recursos humanos, tecnologías de la información, compras y administración, en lo que respecta a la información de los procesos anteriores.

### 2.2 Ubicaciones
| Sede | Dirección | Actividades |
|---|---|---|
| [Oficina central] | [Dirección] | [Actividades] |
| Trabajo remoto | Domicilios de colaboradores autorizados | Todas las actividades del alcance, conforme a POL-08 |

### 2.3 Tecnología
| Componente | Descripción | Gestionado por |
|---|---|---|
| Correo y colaboración | [Ejemplo: Microsoft 365] | [Interno / Proveedor] |
| Infraestructura en la nube | [Ejemplo: AWS, región us-east-1] | [Interno / Proveedor] |
| Aplicaciones de negocio | [Ejemplo: CRM, ERP] | [Interno / Proveedor] |
| Equipos de usuario | [Ejemplo: laptops corporativas con Windows 11] | Interno |
| Red local | [Ejemplo: red de oficina y wifi corporativa] | Interno |

### 2.4 Personas
Todo el personal, interno y externo, que accede a la información de los procesos incluidos.

## 3. Exclusiones

| Elemento excluido | Justificación |
|---|---|
| [Ejemplo: la línea de negocio de capacitación presencial] | [Ejemplo: no procesa información de clientes considerada en el alcance y opera con recursos independientes] |

> 💡 Las exclusiones no deben dejar fuera algo de lo que dependan los procesos incluidos. Si tu servicio corre en un centro de datos externo, el centro de datos no se "excluye": se gestiona como proveedor (A.5.19 – A.5.23).

## 4. Interfaces y dependencias

| Interfaz o dependencia | Tipo | Cómo se controla |
|---|---|---|
| [Proveedor de nube] | Externa | Evaluación del proveedor, acuerdos contractuales, revisión de informes SOC 2 o certificaciones |
| [Corporativo, si eres filial] | Interna | Acuerdo de nivel de servicio interno |
| [Proveedor de nómina] | Externa | Contrato con cláusulas de confidencialidad y protección de datos |

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
