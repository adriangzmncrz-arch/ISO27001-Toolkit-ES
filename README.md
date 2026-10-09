# ISO 27001 Toolkit en español

**Plantillas listas para adaptar que te ayudan a implementar un Sistema de Gestión de Seguridad de la Información (SGSI) alineado a ISO/IEC 27001:2022.**

Políticas, procedimientos, Declaración de Aplicabilidad, matriz de riesgos y formatos de registro, escritos en español y pensados para organizaciones pequeñas y medianas de México y Latinoamérica.

[![Licencia: CC BY-SA 4.0](https://img.shields.io/badge/Licencia-CC%20BY--SA%204.0-lightgrey.svg)](LICENSE)
![ISO/IEC 27001:2022](https://img.shields.io/badge/ISO%2FIEC-27001%3A2022-blue)
![Idioma: español](https://img.shields.io/badge/idioma-espa%C3%B1ol-green)

---

## ¿Para quién es?

- **PyMEs** que quieren ordenar su seguridad de la información o prepararse para certificarse.
- **Responsables de SGSI y consultores** que necesitan un punto de partida sólido en lugar de una hoja en blanco.
- **Estudiantes y auditores en formación** que quieren ver cómo se ve un SGSI documentado de principio a fin.

## ¿Qué incluye?

| Carpeta | Contenido | Cláusulas / controles |
|---|---|---|
| [`01-contexto-y-alcance/`](01-contexto-y-alcance/) | Contexto de la organización, partes interesadas, alcance del SGSI, roles y responsabilidades | 4.1 – 4.3, 5.3 |
| [`02-politicas/`](02-politicas/) | Política general de seguridad y 10 políticas temáticas | 5.2, A.5 – A.8 |
| [`03-procedimientos/`](03-procedimientos/) | Riesgos, incidentes, control documental, auditoría interna, acciones correctivas, cambios, accesos y revisión por la dirección | 6.1, 7.5, 8, 9, 10 |
| [`04-declaracion-aplicabilidad/`](04-declaracion-aplicabilidad/) | SoA con los 93 controles del Anexo A en Excel y CSV | 6.1.3 d) |
| [`05-gestion-riesgos/`](05-gestion-riesgos/) | Matriz de riesgos con cálculo automático, catálogos de amenazas y vulnerabilidades | 6.1.2, 6.1.3, 8.2, 8.3 |
| [`06-registros/`](06-registros/) | Formatos: objetivos, programa e informe de auditoría, reporte de incidente, acta de revisión, no conformidades, competencias | 6.2, 7.2, 9.2, 9.3, 10.2 |
| [`docs/`](docs/) | Guía de uso, mapa de información documentada obligatoria y glosario | — |

> 📌 Consulta el [**mapa documental**](docs/mapa-documental.md) para ver qué exige la norma como información documentada y qué plantilla la cubre.

## Inicio rápido

1. **Haz fork o descarga** el repositorio (`Code → Download ZIP`).
2. **Reemplaza los marcadores**: todos los datos a personalizar están entre corchetes, por ejemplo `[NOMBRE DE LA ORGANIZACIÓN]`, `[RESPONSABLE DEL SGSI]`. Busca `[` en tu editor.
3. **Sigue el orden recomendado** de la [guía de uso](docs/guia-de-uso.md): primero contexto y alcance, luego riesgos, después la SoA y al final las políticas y procedimientos que resulten aplicables.
4. **Elimina lo que no aplique.** Una plantilla que no refleja tu operación real es un hallazgo de auditoría esperando a ocurrir.

## Principios del toolkit

- **Adaptable, no genérico.** Cada documento indica qué decisiones debes tomar tú.
- **Proporcional.** Pensado para organizaciones de 10 a 500 personas; nada de burocracia innecesaria.
- **Trazable.** Cada documento indica las cláusulas y controles que atiende.
- **Contexto mexicano.** Referencias a la LFPDPPP (2025) y a prácticas locales donde aplica.

## Aviso importante

- Este toolkit **no reproduce el texto de la norma ISO/IEC 27001**. Los nombres de los controles son traducciones libres de referencia. Para implementar y certificarte necesitas la norma oficial, disponible en [ISO](https://www.iso.org/standard/27001) o en organismos nacionales de normalización.
- Usar estas plantillas **no garantiza la certificación**. Un SGSI funciona cuando refleja lo que la organización realmente hace.
- Las referencias legales son informativas y **no constituyen asesoría legal**.

## Hoja de ruta

- [x] v1.0 — Políticas, procedimientos, SoA, matriz de riesgos y formatos
- [ ] Plan de continuidad del negocio y BIA (vínculo con ISO 22301)
- [ ] Mapeo de controles a NIST CSF 2.0 y CIS Controls v8
- [ ] Checklist de auditoría interna por cláusula y control
- [ ] Versión en formato Word (.docx) de cada plantilla

¿Te gustaría ver algo más? [Abre un issue](../../issues/new/choose).

## Contribuir

Las contribuciones son bienvenidas: correcciones, mejoras de redacción, nuevas plantillas o adaptaciones para otros países. Lee [CONTRIBUTING.md](CONTRIBUTING.md) antes de enviar un pull request.

## Licencia

Contenido bajo [Creative Commons Atribución-CompartirIgual 4.0 Internacional (CC BY-SA 4.0)](LICENSE). Puedes usarlo, adaptarlo y usarlo comercialmente, incluso con tus clientes, siempre que des crédito y compartas tus versiones derivadas públicas bajo la misma licencia. **Los documentos internos que generes para tu organización a partir de estas plantillas no necesitan publicarse.**

## Autor

**Carlos Adrián Guzmán** — Consultor GRC, Lead Auditor ISO 27001 / 9001 / 22301
Director General de [Cipherwell](https://cipherwell-sec.com) · [LinkedIn](https://www.linkedin.com/in/adriancruz-grc/)

¿Necesitas ayuda para implementar tu SGSI o prepararte para la auditoría de certificación? [Contáctanos](https://cipherwell-sec.com).

---

⭐ Si este toolkit te resulta útil, dale una estrella al repositorio. Ayuda a que más personas lo encuentren.
