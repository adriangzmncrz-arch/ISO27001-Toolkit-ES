# Procedimiento de Gestión de Accesos de Usuarios

| Campo | Valor |
|---|---|
| Código | PRO-07 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DE TI] |
| Aprobó | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.5.11, A.5.16, A.5.18, A.6.1, A.6.2, A.6.5, A.6.6 |

> 💡 **Cómo adaptar:** si usas un directorio central (Entra ID, Google Workspace) y un esquema de inicio de sesión único (SSO), la mayoría de las bajas se resuelven deshabilitando una sola cuenta. Identifica las aplicaciones que **no** están integradas al SSO: son las que se olvidan.

## 1. Propósito

Controlar el ciclo de vida de las identidades y sus accesos: altas, cambios de puesto y bajas.

## 2. Alta de personal

| Paso | Actividad | Responsable | Plazo |
|---|---|---|---|
| 1 | Verificación de antecedentes conforme a la legislación y al puesto | RR. HH. | Antes de la contratación |
| 2 | Firma de contrato con cláusulas de confidencialidad y de responsabilidades de seguridad | RR. HH. | Antes del ingreso |
| 3 | Solicitud de alta por ticket indicando puesto, área, jefe y fecha de ingreso | RR. HH. | [3] días hábiles antes del ingreso |
| 4 | Asignación de accesos según el perfil del puesto (matriz de roles) | TI | Antes del ingreso |
| 5 | Accesos adicionales al perfil: autorización del propietario del activo | Jefe inmediato / Propietario | Por solicitud |
| 6 | Entrega de equipo y credenciales iniciales por canal seguro; registro de MFA | TI | Día de ingreso |
| 7 | Firma de la carta de aceptación de POL-02 y concientización inicial | RR. HH. / Resp. SGSI | Primera semana |

## 3. Cambio de puesto

1. RR. HH. notifica el cambio por ticket con [3] días hábiles de anticipación.
2. TI asigna los accesos del nuevo perfil y **retira los que ya no correspondan** en un máximo de [5] días hábiles tras el cambio.
3. Se evita la acumulación de permisos: el perfil anterior no se conserva "por si acaso".

## 4. Baja de personal

| Paso | Actividad | Responsable | Plazo |
|---|---|---|---|
| 1 | Notificación de baja por ticket con fecha y hora efectiva | RR. HH. | En cuanto se conozca; en bajas no voluntarias, antes de la notificación al colaborador |
| 2 | Deshabilitar la cuenta del directorio y revocar sesiones activas | TI | A la hora efectiva |
| 3 | Revocar accesos en aplicaciones no integradas al SSO, VPN, accesos físicos y certificados | TI | Mismo día |
| 4 | Cambiar contraseñas de cuentas compartidas o de servicio que conocía la persona | TI | Mismo día |
| 5 | Recuperar activos: equipo, tarjetas, tokens, documentos (A.5.11) | RR. HH. / TI | Último día |
| 6 | Transferir buzón y archivos al jefe inmediato según las indicaciones | TI | [30] días |
| 7 | Recordar las obligaciones de confidencialidad vigentes tras la salida | RR. HH. | Último día |
| 8 | Eliminar la cuenta | TI | Tras [30-90] días |

## 5. Contratistas y terceros

- Sus cuentas tienen **fecha de expiración** igual al término del contrato o, como máximo, de [6] meses renovables.
- El responsable interno del contrato solicita y justifica el acceso.
- Firman acuerdo de confidencialidad antes de recibir accesos (A.6.6).

## 6. Revisión periódica de accesos

Conforme a POL-01, sección 7. Adicionalmente, cada [mes] se cruza la lista de personal activo de RR. HH. con las cuentas activas del directorio y de las aplicaciones críticas para detectar cuentas huérfanas.

## 7. Registros

- Tickets de alta, cambio y baja.
- Evidencia de revisiones de acceso y de los ajustes realizados.
- Constancias de devolución de activos.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
