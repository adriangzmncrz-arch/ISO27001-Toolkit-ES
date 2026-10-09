# Política de Trabajo Remoto y Dispositivos Móviles

| Campo | Valor |
|---|---|
| Código | POL-08 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [RESPONSABLE DEL SGSI] |
| Aprobó | [DIRECCIÓN GENERAL] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.6.7, A.7.8, A.7.9, A.8.1 |

> 💡 **Cómo adaptar:** en México, la NOM-037-STPS-2023 regula condiciones de teletrabajo en materia de seguridad y salud. Coordina esta política con Recursos Humanos para que sea coherente con los contratos y las políticas laborales de teletrabajo.

## 1. Propósito

Proteger la información a la que se accede, que se procesa o se almacena fuera de las instalaciones de la organización y en dispositivos móviles.

## 2. Equipos autorizados

| Tipo de dispositivo | Acceso permitido |
|---|---|
| Laptop corporativa gestionada | Todos los sistemas según el rol |
| Teléfono corporativo gestionado por MDM | Correo, colaboración, aplicaciones autorizadas |
| Teléfono personal (BYOD) con perfil de trabajo o MAM | Correo y colaboración; sin descarga local de información Confidencial |
| Computadora personal | [Solo acceso vía navegador a [SERVICIOS] / No permitido] |

## 3. Requisitos de los dispositivos

Todo dispositivo que acceda a información de la organización debe tener:
- Sistema operativo con soporte vigente del fabricante y actualizaciones automáticas.
- Bloqueo de pantalla con PIN de al menos 6 dígitos, contraseña o biometría.
- Cifrado del almacenamiento (POL-06).
- En dispositivos corporativos: antimalware/EDR gestionado y firewall activo.
- Capacidad de borrado remoto de la información corporativa.

## 4. Reglas para el trabajo remoto

1. Conectarse por [VPN / acceso de confianza cero] a los sistemas internos que lo requieran.
2. No usar redes wifi públicas sin VPN; preferir compartir datos del teléfono.
3. Cambiar la contraseña predeterminada del módem o *router* doméstico y usar cifrado WPA2 o WPA3.
4. Trabajar en un espacio donde terceros no puedan ver la pantalla ni escuchar llamadas confidenciales.
5. No permitir que familiares u otras personas usen los equipos corporativos.
6. No imprimir información Confidencial en casa, salvo autorización; en ese caso, destruirla de forma segura.
7. Trabajar desde el extranjero requiere autorización previa del Responsable del SGSI.

## 5. Pérdida o robo

Reportar de inmediato a [CANAL DE REPORTE] la pérdida o robo de cualquier dispositivo. TI bloqueará las cuentas y ejecutará el borrado remoto. Se gestiona como incidente conforme a PRO-02.

## 6. Privacidad en BYOD

En dispositivos personales, la organización gestiona únicamente el perfil de trabajo o las aplicaciones corporativas. No accede a fotografías, mensajes ni aplicaciones personales. El borrado remoto en BYOD elimina solo la información corporativa.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
