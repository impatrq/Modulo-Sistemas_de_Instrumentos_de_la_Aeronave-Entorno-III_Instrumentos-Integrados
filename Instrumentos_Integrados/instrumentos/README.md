# Instrumentos Integrados — Manual de 7mo año

Manual de **Instrumentos Integrados (Instrumentos Digitales PFD / MFD)**, parte del módulo **Sistemas de Instrumentos de la Aeronave** (7mo año, Tecnicatura en Aviónica) del **Diseño Curricular 2025** de la Provincia de Buenos Aires. Se dicta en la **E.E.S.T. N° 7 "Taller Regional Quilmes" (IMPA)**, Quilmes, Provincia de Buenos Aires.

Está escrito en **LaTeX** y pensado para compilarse en [Overleaf](https://www.overleaf.com) o en cualquier instalación local de TeX. Edición **Ciclo Lectivo 2026**.

**Autor y docente:** Técnico Aviónico Julián Scicolone — scicolonejulian@impatrq.com

---

## Objetivo

Que el futuro técnico aviónico conozca los instrumentos integrados de pantalla (G1000, G5000, G5, GI 275, G3X Touch, G500/G600 TXi, AXIS, Aspen) y domine el oficio que permite instalarlos: cables aeronáuticos, terminales y crimpado, conectores militares y D-sub, herramientas, ferretería, configuración y ensayos.

La **Hoja de ruta del estudiante** lista los 16 logros del año, que cierra con un **proyecto integrador**: un panel didáctico con su mazo de cables.

---

## Contenido

| Archivo | Sección |
|---|---|
| `caratula.tex` | Carátula |
| `presentacion.tex` | Presentación, fundamentación, objetivos, organización, seguridad y hoja de ruta |
| `u1_glass.tex` | **Unidad 1 – La cabina de cristal:** T básica, EFIS, arquitecturas, normas y certificación |
| `u2_sensores.tex` | **Unidad 2 – Sensores y buses de datos:** pitot-estático, ADC, AHRS, magnetómetro, sensores de motor, ARINC 429, CAN, Ethernet |
| `u3_pfd_mfd.tex` | **Unidad 3 – El PFD y el MFD:** presentación, alertas, banderas, modos reversionarios, reserva |
| `u4_g1000.tex` | **Unidad 4 – Sistemas integrados:** G1000 / NXi, G3000 / G5000, configuración y bases de datos |
| `u5_retrofit.tex` | **Unidad 5 – Equipos de reemplazo:** G5, GI 275, Aspen, G3X Touch, G500/G600 TXi, AXIS |
| `u6_cables.tex` | **Unidad 6 – Cables aeronáuticos:** tipos, sección y caída de tensión, identificación, mazos, blindajes, masas, EWIS |
| `u7_crimpado.tex` | **Unidad 7 – Terminales y crimpado:** pelado, terminales, crimpadoras M22520, inspección, tracción, soldadura |
| `u8_conectores.tex` | **Unidad 8 – Conectores:** D-sub, MIL-DTL-38999 y otros circulares, contactos, inserción y extracción |
| `u9_herramientas.tex` | **Unidad 9 – Herramientas y ferretería:** herramental, instrumentos, protecciones, ferretería AN/MS/NAS, trazabilidad |
| `u10_instalacion.tex` | **Unidad 10 – Instalación de un panel digital:** planificación, panel, plano de cableado, mazo, configuración, documentación |
| `u11_ensayos.tex` | **Unidad 11 – Ensayos y diagnóstico:** pitot-estático, chequeos funcionales, fallas típicas, tarjeta de trabajo |
| `practicas.tex` | Trabajos prácticos de taller (8 TPs) |
| `proyecto_panel.tex` | Proyecto integrador: panel didáctico con su mazo de cables |

Recursos: `logos/` — logos de la Provincia de Buenos Aires y de IMPA (PDF).

---

## Cómo compilar

### En Overleaf

1. Descargar el repositorio como `.zip` (botón **Code → Download ZIP**).
2. En Overleaf: **New Project → Upload Project** y elegir el zip.
3. Verificar que el compilador sea **pdfLaTeX** (Menu → Compiler).
4. Compilar `main.tex`.

### En una instalación local

```bash
pdflatex main.tex
pdflatex main.tex   # segunda pasada para referencias
```

Paquetes utilizados: `lmodern`, `babel` (spanish), `geometry`, `graphicx`, `tikz`, `xcolor`, `enumitem`, `fancyhdr`, `microtype`, `array`, `titlesec`, `tcolorbox`.

---

## Cómo modificarlo

- Cada unidad está en su propio archivo `.tex`. Para quitar o reordenar una unidad, comentá o mové su línea `\input{...}` en `main.tex`.
- El encabezado y el pie se definen en `main.tex` (estilo `materia`).
- Los recuadros destacados usan el entorno `recuadro`; las casillas de la hoja de ruta, el comando `\casilla`.

---

## Datos que conviene revisar cada año

- Requisitos de ensayos pitot-estáticos, de altímetro y de transpondedor en las **RAAC** vigentes.
- Equipos y STC disponibles (y su aceptación por la ANAC); la línea de productos cambia rápido.
- Números de parte y procedimientos: siempre del manual de instalación vigente del fabricante.

---

## Créditos

- Contenidos y edición: **Téc. Aviónico Julián Scicolone**.
- Programa basado en el Diseño Curricular 2025 (IF-2025-41581603-GDEBA-DETECDGCYE).
- E.E.S.T. N° 7 "Taller Regional Quilmes" — Dirección General de Cultura y Educación de la Provincia de Buenos Aires.
