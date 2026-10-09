# Cómo contribuir

¡Gracias por tu interés! Este toolkit mejora con la experiencia de quienes implementan y auditan SGSI en la práctica.

## Formas de contribuir

- **Reportar errores**: referencias incorrectas a cláusulas o controles, enlaces rotos, errores de redacción.
- **Proponer mejoras**: redacción más clara, controles faltantes, ejemplos más útiles.
- **Nuevas plantillas**: documentos que te hayan funcionado en implementaciones reales.
- **Adaptaciones por país**: referencias a la legislación de tu país (Colombia, Chile, Perú, España, etc.).

## Proceso

1. Abre un *issue* describiendo el cambio, salvo que sea una corrección menor.
2. Haz *fork* del repositorio y crea una rama descriptiva: `mejora/politica-respaldo`, `fix/soa-control-8-12`.
3. Realiza tus cambios respetando las convenciones de abajo.
4. Abre un *pull request* usando la plantilla.

## Convenciones

**Formato**
- Documentos en Markdown (`.md`); hojas de cálculo en `.xlsx` con un `.csv` equivalente cuando sea posible, para que los cambios se puedan revisar en GitHub.
- Cada documento comienza con la tabla de control documental (código, versión, propietario, etc.).
- Datos a personalizar entre corchetes y en mayúsculas: `[NOMBRE DE LA ORGANIZACIÓN]`.

**Códigos**
| Prefijo | Tipo |
|---|---|
| `DOC-` | Documentos de contexto y alcance |
| `POL-` | Políticas |
| `PRO-` | Procedimientos |
| `REG-` | Formatos de registro |

**Redacción**
- Español neutro, claro y directo. Evita anglicismos cuando exista un término en español de uso común.
- Usa "debe" para requisitos obligatorios y "se recomienda" para buenas prácticas.
- Indica siempre la cláusula o control de ISO/IEC 27001:2022 que atiende el documento.

**Derechos de autor**
- **No copies texto de las normas ISO**, ni de otros toolkits o materiales con derechos reservados. Redacta con tus propias palabras.
- Al contribuir aceptas que tu aporte se publique bajo la licencia CC BY-SA 4.0 del repositorio.

## Código de conducta

Trato respetuoso y constructivo. Las discusiones técnicas se centran en el contenido, no en las personas.
