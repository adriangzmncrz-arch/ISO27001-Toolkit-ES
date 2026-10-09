# Política de Uso de Criptografía

| Campo | Valor |
|---|---|
| Código | POL-06 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DE TI] |
| Aprobó | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.8.24, A.5.31, A.5.33, A.8.20, A.8.21 |

> 💡 **Cómo adaptar:** revisa esta tabla cada año. Los algoritmos aceptables cambian y la criptografía poscuántica empezará a aparecer en requisitos de clientes y reguladores en los próximos años.

## 1. Propósito

Asegurar el uso adecuado y eficaz de la criptografía para proteger la confidencialidad, autenticidad e integridad de la información.

## 2. Cuándo se cifra

| Escenario | Requisito |
|---|---|
| Laptops y equipos de escritorio | Cifrado de disco completo obligatorio (BitLocker, FileVault o equivalente) |
| Dispositivos móviles con información corporativa | Cifrado del dispositivo activado y gestionado por MDM |
| Medios removibles con información Confidencial o Restringida | Cifrado obligatorio |
| Bases de datos y almacenamiento en la nube | Cifrado en reposo habilitado |
| Respaldos | Cifrado en tránsito y en reposo |
| Tráfico web y API | TLS 1.2 como mínimo; se recomienda TLS 1.3 |
| Acceso remoto | VPN o acceso de confianza cero con cifrado fuerte |
| Correo con información Restringida | Cifrado de mensaje o enlace seguro |
| Contraseñas almacenadas en aplicaciones propias | Funciones de derivación específicas (Argon2id, bcrypt, scrypt); nunca cifrado reversible ni hash simple |

## 3. Algoritmos

| Uso | Aceptados | Prohibidos |
|---|---|---|
| Cifrado simétrico | AES-256 (GCM recomendado), AES-128, ChaCha20-Poly1305 | DES, 3DES, RC4, AES en modo ECB |
| Cifrado asimétrico y firma | RSA de 3072 bits o más, ECDSA/EdDSA (P-256, Ed25519 o superior) | RSA menor a 2048 bits |
| Hash | SHA-256, SHA-384, SHA-512, SHA-3 | MD5, SHA-1 |
| Protocolos | TLS 1.2 con suites seguras, TLS 1.3, SSH v2 | SSL, TLS 1.0, TLS 1.1 |

## 4. Gestión de llaves y certificados

1. Las llaves se generan con fuentes de aleatoriedad seguras y en el sistema que las usará o en un servicio de gestión de llaves (KMS, HSM).
2. Las llaves privadas y secretos se almacenan en [GESTOR DE SECRETOS / KMS]. Nunca en código fuente, correos o documentos.
3. Las llaves se rotan [anualmente] o de inmediato ante sospecha de compromiso.
4. Se mantiene un inventario de certificados con su fecha de expiración y se alerta con al menos [30] días de anticipación.
5. Se usan certificados emitidos por autoridades certificadoras reconocidas para servicios públicos.
6. Al dar de baja una llave, se revoca y se destruye de forma segura.

## 5. Cumplimiento legal

El uso de criptografía debe cumplir las leyes del país donde se usa. Antes de enviar equipos o software con cifrado a otros países, se verifican las restricciones de importación o exportación aplicables.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
