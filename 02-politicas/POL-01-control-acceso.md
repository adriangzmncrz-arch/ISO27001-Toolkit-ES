# Política de Control de Acceso

| Campo | Valor |
|---|---|
| Código | POL-01 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DE TI] |
| Aprobó | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.5.15, A.5.16, A.5.17, A.5.18, A.8.2, A.8.3, A.8.4, A.8.5 |

> 💡 **Cómo adaptar:** ajusta los plazos de revisión y los requisitos de contraseña a lo que tus sistemas permiten técnicamente. Si un sistema heredado no soporta MFA, documenta la excepción y el control compensatorio.

## 1. Propósito

Asegurar que el acceso a la información y a los sistemas se otorgue únicamente a personas autorizadas, con base en la necesidad de conocer y el mínimo privilegio.

## 2. Alcance

Todos los sistemas, aplicaciones, redes, servicios en la nube e información dentro del alcance del SGSI, y todas las identidades que accedan a ellos: personal, contratistas, proveedores y cuentas de servicio.

## 3. Principios

- **Necesidad de conocer:** solo se accede a la información requerida para las funciones del puesto.
- **Mínimo privilegio:** se otorgan los permisos mínimos necesarios, por el tiempo necesario.
- **Identidad única:** cada persona usa una cuenta nominal. Las cuentas compartidas están prohibidas, salvo excepción aprobada y registrada.
- **Denegación por defecto:** todo acceso no autorizado expresamente está prohibido.
- **Segregación de funciones:** conforme a DOC-03.

## 4. Gestión de identidades y accesos

1. Las altas, modificaciones y bajas siguen el procedimiento PRO-07.
2. Todo acceso requiere la autorización del propietario del activo.
3. Los accesos se otorgan preferentemente por **roles o grupos**, no a usuarios individuales.
4. Las bajas de personal se ejecutan **el mismo día** en que termina la relación laboral; en salidas no voluntarias, antes de la notificación al colaborador.
5. Las cuentas inactivas por más de **[90] días** se deshabilitan.
6. Las cuentas de servicio tienen un propietario asignado, no permiten inicio de sesión interactivo cuando sea técnicamente posible y sus credenciales se resguardan en [GESTOR DE SECRETOS].

## 5. Accesos privilegiados (A.8.2)

1. Los administradores usan una cuenta privilegiada **separada** de su cuenta de uso diario.
2. Las cuentas privilegiadas requieren MFA en todos los casos.
3. El número de administradores globales o *root* se limita a [2-3] personas.
4. Se registran las actividades de las cuentas privilegiadas y se revisan [mensualmente].
5. Se prefiere el acceso privilegiado **justo a tiempo** cuando la plataforma lo permita.

## 6. Autenticación (A.5.17, A.8.5)

| Requisito | Estándar |
|---|---|
| MFA | Obligatorio para correo, acceso remoto, nube, aplicaciones críticas y cuentas privilegiadas |
| Longitud mínima de contraseña | 12 caracteres para usuarios; 16 para cuentas privilegiadas y de servicio |
| Complejidad | Se recomiendan frases de contraseña; se bloquean contraseñas comunes o filtradas |
| Cambio de contraseña | Solo ante sospecha de compromiso, no por calendario |
| Bloqueo | Tras [10] intentos fallidos o mecanismo equivalente de limitación |
| Gestor de contraseñas | [NOMBRE DEL GESTOR] autorizado para uso corporativo |
| Contraseñas iniciales | Únicas, entregadas por canal seguro y con cambio obligatorio en el primer inicio |

> 💡 Este enfoque sigue las recomendaciones actuales (por ejemplo, NIST SP 800-63B), que desaconsejan el cambio periódico forzado de contraseñas.

## 7. Revisión de accesos (A.5.18)

| Tipo de acceso | Frecuencia | Responsable |
|---|---|---|
| Cuentas privilegiadas | Trimestral | Responsable de TI y Responsable del SGSI |
| Aplicaciones críticas | Semestral | Propietario del activo |
| Resto de los sistemas | Anual | Propietario del activo |

La revisión se documenta con la lista revisada, los cambios solicitados y la evidencia de su ejecución.

## 8. Acceso a código fuente (A.8.4)

El acceso de escritura a repositorios de código se limita al equipo de desarrollo autorizado. Las ramas principales están protegidas y requieren revisión antes de integrar cambios (ver POL-07).

## 9. Excepciones

Las excepciones se solicitan por escrito al Responsable del SGSI, indican el riesgo, el control compensatorio y la fecha de vencimiento, y se registran en el registro de excepciones.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
