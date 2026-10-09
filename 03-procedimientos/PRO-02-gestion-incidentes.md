# Procedimiento de Gestión de Incidentes de Seguridad de la Información

| Campo | Valor |
|---|---|
| Código | PRO-02 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.5.5, A.5.24, A.5.25, A.5.26, A.5.27, A.5.28, A.6.8 |

> 💡 **Cómo adaptar:** el anexo de contactos es lo que más se usa durante un incidente real, y lo que menos se mantiene. Llénalo, imprímelo y guárdalo también fuera de tus sistemas: si el incidente es un *ransomware*, quizá no puedas abrir este documento.

## 1. Propósito

Asegurar una respuesta rápida, eficaz y ordenada ante eventos e incidentes de seguridad de la información, minimizando su impacto y aprendiendo de ellos.

## 2. Equipo de respuesta a incidentes

| Rol | Persona | Suplente |
|---|---|---|
| Coordinador del incidente | [RESPONSABLE DEL SGSI] | [NOMBRE] |
| Líder técnico | [RESPONSABLE DE TI] | [NOMBRE] |
| Comunicación | [DIRECCIÓN / COMUNICACIÓN] | [NOMBRE] |
| Legal y datos personales | [ASESOR LEGAL] | [NOMBRE] |
| Dirección | [DIRECCIÓN GENERAL] | [NOMBRE] |

## 3. Reporte (A.6.8)

Toda persona que detecte o sospeche un evento de seguridad lo reporta **de inmediato** por:
- Correo: [seguridad@empresa.com]
- Teléfono o mensajería: [NÚMERO]
- Botón de reporte de *phishing* en el cliente de correo

No se debe intentar investigar por cuenta propia, apagar equipos ni borrar evidencia. Si se sospecha que un equipo está comprometido, **desconectarlo de la red** (cable o wifi) sin apagarlo.

## 4. Clasificación y severidad (A.5.25)

| Severidad | Criterio | Ejemplos | Tiempo de respuesta | Escalamiento |
|---|---|---|---|---|
| **S1 — Crítica** | Afecta servicios críticos, datos Restringidos o a muchos clientes; riesgo legal o reputacional grave | *Ransomware*, fuga masiva de datos, compromiso de cuenta de administrador | Inmediato (< 1 h), 24/7 | Dirección General de inmediato |
| **S2 — Alta** | Afecta información Confidencial o un servicio importante de forma limitada | Cuenta de usuario comprometida con acceso a datos de clientes, malware en servidor | < 4 h | Responsable del SGSI |
| **S3 — Media** | Impacto limitado y contenido | Malware detenido por EDR, pérdida de laptop cifrada | < 1 día hábil | Responsable de TI |
| **S4 — Baja** | Evento sin impacto confirmado | *Phishing* reportado sin interacción, escaneo externo | < 3 días hábiles | No requiere |

## 5. Fases de respuesta (A.5.26)

```
Detección y reporte → Análisis y clasificación → Contención → Erradicación → Recuperación → Lecciones aprendidas
```

### 5.1 Análisis y clasificación
- Registrar el incidente en [HERRAMIENTA / REG-04] con número consecutivo.
- Confirmar si es un incidente, determinar alcance, activos y datos afectados.
- Asignar severidad y convocar al equipo según la tabla.

### 5.2 Contención
- **Corto plazo:** aislar equipos, deshabilitar cuentas, bloquear direcciones o dominios, revocar sesiones y tokens.
- **Largo plazo:** aplicar cambios temporales que permitan operar mientras se erradica la causa.

### 5.3 Recolección de evidencia (A.5.28)
- Preservar bitácoras, imágenes de memoria o disco y correos antes de modificar los sistemas, cuando el incidente pueda tener consecuencias legales o disciplinarias.
- Documentar la cadena de custodia: qué se recolectó, quién, cuándo, cómo y dónde se resguarda.
- Si se requiere análisis forense especializado, contactar a [PROVEEDOR DE RESPUESTA A INCIDENTES].

### 5.4 Erradicación y recuperación
- Eliminar la causa raíz: malware, persistencias, cuentas creadas por el atacante, vulnerabilidades explotadas.
- Restaurar desde respaldos verificados (POL-05).
- Restablecer credenciales afectadas.
- Monitorear de forma reforzada durante [14] días.

### 5.5 Lecciones aprendidas (A.5.27)
Para incidentes S1 y S2, en un máximo de [10] días hábiles después del cierre:
- Sesión de revisión sin culpables: ¿qué pasó?, ¿qué funcionó?, ¿qué no?, ¿qué cambiamos?
- Las acciones de mejora se registran como acciones correctivas (PRO-05).
- Se actualiza la evaluación de riesgos si corresponde.

## 6. Notificaciones

| Destinatario | Cuándo | Responsable |
|---|---|---|
| Dirección General | S1 de inmediato; S2 en el mismo día | Coordinador |
| Clientes afectados | Según contrato, generalmente en [24-72] h | Dirección / Comunicación |
| Titulares de datos personales | Cuando la vulneración afecte de forma significativa sus derechos, conforme a POL-10 | Legal |
| Aseguradora (ciberseguro) | Según la póliza, usualmente de inmediato | Dirección |
| Autoridades (Policía Cibernética, Fiscalía) | Cuando haya un posible delito | Legal |
| CERT-MX | Cuando aporte valor o se requiera apoyo | Coordinador |

## 7. Playbooks rápidos

### Phishing con credenciales capturadas
1. Restablecer la contraseña y revocar todas las sesiones activas.
2. Verificar y reforzar MFA; revisar métodos de MFA registrados por el atacante.
3. Revisar reglas de reenvío y buzón creadas recientemente.
4. Buscar el mismo correo en otros buzones y eliminarlo.
5. Revisar los accesos de la cuenta en los últimos [30] días.

### Ransomware
1. Aislar de la red los equipos afectados **sin apagarlos**.
2. Deshabilitar cuentas privilegiadas posiblemente comprometidas.
3. Verificar la integridad de los respaldos inmutables antes de cualquier restauración.
4. Escalar a S1, notificar a la aseguradora y contactar al proveedor de respuesta.
5. No contactar a los atacantes ni pagar rescates sin decisión de la Dirección General y asesoría legal.

### Pérdida o robo de equipo
1. Confirmar si el equipo estaba cifrado.
2. Ejecutar el borrado remoto y revocar sesiones y certificados del dispositivo.
3. Restablecer credenciales almacenadas en el equipo.
4. Levantar denuncia si fue robo y conservar el número de folio.

### Fraude por suplantación de correo (BEC)
1. Contactar de inmediato al banco para intentar detener o revertir la transferencia.
2. Preservar los correos con encabezados completos.
3. Verificar si la cuenta de correo propia fue comprometida (playbook de *phishing*).
4. Avisar al cliente o proveedor suplantado.

## Anexo A — Contactos de emergencia

| Contacto | Nombre | Teléfono | Correo |
|---|---|---|---|
| Proveedor de respuesta a incidentes | [ ] | [ ] | [ ] |
| Aseguradora (ciberseguro) — póliza [ ] | [ ] | [ ] | [ ] |
| Proveedor de internet | [ ] | [ ] | [ ] |
| Proveedor de nube / soporte | [ ] | [ ] | [ ] |
| Banco — línea de fraudes | [ ] | [ ] | [ ] |
| Asesor legal | [ ] | [ ] | [ ] |
| Policía Cibernética estatal | [ ] | [ ] | [ ] |
| CERT-MX | [ ] | [ ] | [ ] |

> Verifica los datos de contacto de autoridades al llenar este anexo y al menos una vez al año, porque cambian con frecuencia.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
