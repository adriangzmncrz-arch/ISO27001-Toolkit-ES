# Política de Desarrollo Seguro

| Campo | Valor |
|---|---|
| Código | POL-07 |
| Versión | 1.0 |
| Fecha de emisión | [AAAA-MM-DD] |
| Propietario | [LÍDER DE DESARROLLO] |
| Aprobó | [RESPONSABLE DEL SGSI] |
| Clasificación | Uso interno |
| Referencias ISO/IEC 27001:2022 | A.8.4, A.8.25, A.8.26, A.8.27, A.8.28, A.8.29, A.8.30, A.8.31, A.8.32, A.8.33 |

> 💡 **Cómo adaptar:** si tu organización no desarrolla software, puedes excluir esta política y los controles A.8.25 a A.8.31 en la SoA, justificándolo. Si solo hace configuraciones o automatizaciones menores, simplifica la sección 4. Si el desarrollo es externo, conserva la sección 6.

## 1. Propósito

Integrar la seguridad en todo el ciclo de vida del desarrollo de software y sistemas.

## 2. Alcance

Aplicaciones, servicios, API, infraestructura como código, *scripts* y automatizaciones desarrollados interna o externamente para la organización o sus clientes.

## 3. Requisitos de seguridad (A.8.26)

Desde la fase de diseño se identifican los requisitos de seguridad de cada desarrollo, considerando:
- Clasificación de la información que procesará.
- Autenticación, autorización y gestión de sesiones.
- Registro de eventos de seguridad.
- Protección de datos personales desde el diseño.
- Requisitos legales y contractuales del cliente.

Para cambios significativos se realiza un modelado de amenazas ligero (por ejemplo, STRIDE).

## 4. Ciclo de desarrollo

| Fase | Control mínimo |
|---|---|
| Diseño | Requisitos de seguridad documentados; modelado de amenazas para funcionalidades críticas |
| Codificación (A.8.28) | Lineamientos de codificación segura basados en OWASP; prohibido incluir secretos en el código |
| Control de versiones (A.8.4) | Repositorios privados; rama principal protegida; *commits* firmados recomendados |
| Revisión | Revisión de código por al menos una persona distinta del autor antes de integrar a la rama principal |
| Análisis automatizado | SAST, análisis de dependencias (SCA) y detección de secretos en el *pipeline* de integración continua |
| Pruebas (A.8.29) | Pruebas de seguridad antes de liberar; DAST o prueba de penetración para aplicaciones expuestas a internet [anualmente / en cada versión mayor] |
| Liberación (A.8.32) | Cambio aprobado conforme a PRO-06 |

## 5. Ambientes (A.8.31, A.8.33)

1. Los ambientes de desarrollo, pruebas y producción están separados.
2. Los desarrolladores no tienen acceso de escritura a producción salvo excepción aprobada y registrada.
3. **No se usan datos personales ni información Confidencial de producción en ambientes de pruebas.** Si es indispensable, se anonimizan o enmascaran previamente.
4. Los secretos se gestionan por ambiente y nunca se comparten entre producción y no producción.

## 6. Dependencias y componentes de terceros

- Se usan solo librerías de fuentes confiables y con mantenimiento activo.
- Las vulnerabilidades críticas en dependencias se atienden según los plazos de POL-09.
- Se mantiene un inventario de componentes (SBOM) para aplicaciones entregadas a clientes [recomendado].

## 7. Desarrollo externo (A.8.30)

Los contratos con desarrolladores externos incluyen: cumplimiento de esta política, propiedad del código, derecho de revisión, entrega de resultados de pruebas de seguridad, y uso de repositorios controlados por la organización.

## Control de cambios

| Versión | Fecha | Descripción | Autor |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | Emisión inicial | [NOMBRE] |
