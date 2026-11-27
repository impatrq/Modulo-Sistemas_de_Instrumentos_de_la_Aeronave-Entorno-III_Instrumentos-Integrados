# Emprendimientos Productivos y Desarrollo Local — Manual de 7mo año

Manual de la materia **Emprendimientos Productivos y Desarrollo Local** (7mo año, Tecnicatura en Aviónica) de la **E.E.S.T. N° 7 "Taller Regional Quilmes" (IMPA)**, Quilmes, Provincia de Buenos Aires.

Está escrito en **LaTeX** y pensado para compilarse en [Overleaf](https://www.overleaf.com) o en cualquier instalación local de TeX. Edición **Ciclo Lectivo 2026**.

**Autor y docente:** Técnico Aviónico Julián Scicolone — scicolonejulian@impatrq.com

---

## Objetivo

La materia busca que el estudiante no solo estudie los contenidos, sino que **egrese con resultados concretos**:

- CV armado y perfil de LinkedIn conectado con sus compañeros.
- Experiencia práctica con un ERP (Odoo) para gestión de stock, almacenes y órdenes de trabajo.
- Capacidad de emitir una factura en ARCA y entender el sistema impositivo argentino.
- Conceptos básicos de comercio exterior, productos bancarios, finanzas y mercado de capitales.
- Un plan de negocios evaluado (punto de equilibrio, VAN, TIR) y presentado en un *pitch*.

La **Hoja de ruta del egresado** (al inicio del manual) lista los 18 logros que cada estudiante tiene que completar durante el año.

---

## Contenido

| Archivo | Sección |
|---|---|
| `caratula.tex` | Carátula |
| `proyecto.tex` | Proyecto pedagógico de la materia |
| `examen.tex` | Modelo de examen final |
| `hoja_ruta.tex` | Hoja de ruta del egresado (checklist de logros) |
| `cuerpo.tex` | Apunte base: la empresa, organización, administración, marketing, RR.HH. (adaptado del material de Ariel Gagliardi) |
| `emprendedorismo.tex` | Emprendedorismo, casos aeronáuticos (FAdeA, Cicaré, Redimec, INVAP), Triángulo de Sabato, sistema científico-tecnológico, desarrollo local, parques industriales, polos tecnológicos y clústeres |
| `plan_negocios.tex` | Laboratorio de ideas, Canvas, plan de negocios, factibilidad (punto de equilibrio, VAN, TIR) y técnicas de comunicación (*pitch*) |
| `impuestos.tex` | Sistema impositivo argentino, monotributo, IVA, facturación en ARCA, comercio exterior e Incoterms, préstamos |
| `sociedades.tex` | Formas jurídicas: monotributista, autónomo, sociedades (SH, SRL, SA, SAS) y cooperativas |
| `banca.tex` | El banco y sus productos: cuentas, tarjetas, homebanking, seguridad |
| `financiacion.tex` | Fuentes de financiamiento (crowdfunding, SGR, inversores) y proceso de compras |
| `practicas.tex` | Prácticas integradoras: importación por courier y comparación de préstamos |
| `mercados.tex` | Mercados financieros y bursátiles: BYMA, A3, riesgo país, bonos, ON, brokers, órdenes, caución, dólar MEP/CCL, futuros, opciones, venta en corto, bolsas del mundo, FCI, ETF, CEDEARs, BCRA y Fed |
| `viaticos.tex` | Viáticos, rendiciones de gastos y caja chica |
| `empleo.tex` | Mi primer empleo: CV, filtros ATS, portales de empleo, LinkedIn, selección de personal, psicotécnicos, networking |
| `sueldo.tex` | Recibo de sueldo, liquidación salarial, aguinaldo, vacaciones y negociación salarial |
| `lean5s.tex` | 5S, Lean Manufacturing y Kaizen |
| `calidad.tex` | ISO 9001, ISO 14001 y análisis FODA |
| `erp.tex` | Sistemas ERP: Odoo, SAP y Salesforce |
| `web.tex` | Presencia digital del proyecto: dominio (NIC Argentina), sitio web, redes, Google Business Profile, Google Ads y Meta Ads |
| `proyecto_odoo.tex` | Proyecto integrador: servidor Odoo para la gestión del pañol |

Recursos:

- `logos/` — logos de la Provincia de Buenos Aires y de IMPA (PDF).
- `figuras/` — imágenes del apunte base.

---

## Cómo compilar

### En Overleaf

1. Descargar el repositorio como `.zip` (botón **Code → Download ZIP**).
2. En Overleaf: **New Project → Upload Project** y elegir el zip.
3. Verificar que el compilador sea **pdfLaTeX** (Menu → Compiler).
4. Compilar `main.tex`.

### En una instalación local

Se necesita una distribución TeX completa (TeX Live o MiKTeX).

```bash
pdflatex main.tex
pdflatex main.tex   # segunda pasada para referencias
```

Paquetes utilizados: `lmodern`, `babel` (spanish), `geometry`, `graphicx`, `tikz`, `xcolor`, `enumitem`, `fancyhdr`, `microtype`, `array`, `titlesec`, `tcolorbox`.

---

## Cómo modificarlo

- Cada unidad o módulo está en su propio archivo `.tex`. Para **quitar o reordenar** un módulo, comentá o mové su línea `\input{...}` en `main.tex`.
- Para **agregar** un módulo nuevo, creá un archivo `.tex` que empiece con `\clearpage` y `\section*{...}`, y sumá su `\input{...}` en `main.tex`.
- El encabezado y el pie de página se definen en `proyecto.tex` (estilo `proyecto`). Para cambiar el año, la materia o el mail, editá el bloque `\fancypagestyle{proyecto}{...}`.
- Los recuadros destacados usan el entorno `recuadro`:

```latex
\begin{recuadro}
Texto destacado.
\end{recuadro}
```

---

## Datos que hay que actualizar cada año

Varios contenidos dependen de normativa y valores que cambian con frecuencia. Antes de cada ciclo lectivo conviene revisar:

- Categorías y montos del **monotributo** y escala de **Ganancias** (ARCA).
- Régimen de **courier** y franquicias de importación.
- Capital mínimo de las sociedades y requisitos de la **SAS**.
- Normativa laboral (Ley 27.802 y su reglamentación), aportes y convenios.
- Datos de mercado: **riesgo país**, tasa de la **Fed**, cantidad de CEDEARs, horarios de BYMA.
- Ejemplos con precios y cotizaciones (son ilustrativos).

El módulo de mercados es de **educación financiera** y no constituye recomendación de inversión.

---

## Créditos

- Apunte base adaptado del material del Prof. **Ariel Gagliardi**, con su autorización.
- Contenidos, módulos nuevos y edición: **Téc. Aviónico Julián Scicolone**.
- E.E.S.T. N° 7 "Taller Regional Quilmes" — Dirección General de Cultura y Educación de la Provincia de Buenos Aires.
