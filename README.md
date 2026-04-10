# IDC — Panel Interactivo de Investigación en Diseño
**Instituto de Diseño y Comunicación · Infografía Académica Interactiva**

---

## Descripción general

Este archivo es un **widget HTML autocontenido** que funciona como panel académico interactivo para el área de Investigación en Diseño del IDC. Integra de forma cohesionada cuatro componentes:

1. **Estructura metodológica cualitativa** basada en el modelo de cuatro partes de Gopaldas (2016) — Frontend, Métodos, Hallazgos y Backend.
2. **Visualizaciones de datos estadísticos** (barras, boxplot, línea de tendencia y diagrama de dispersión) con paleta corporativa IDC.
3. **Tarjetas de investigación aplicada** por carrera: Diseño de Interiores, Diseño Publicitario, Diseño de Modas y Comunicación Audiovisual.
4. **Laboratorio interactivo de gráficos editables** con funciones de restablecimiento y exportación PNG/SVG.

---

## Estructura del archivo

```
output/
└── index_idc_FINAL.html   ← Archivo único autocontenido (HTML + CSS + JS + SVG)
```

Todo el proyecto reside en un **único archivo HTML**. No requiere servidor, frameworks ni dependencias externas más allá de las fuentes cargadas desde Google Fonts y Fontshare vía CDN.

---

## Secciones del documento

| # | Sección | Descripción |
|---|---|---|
| 00 | **Hero IDC** | Logo, badge institucional, título principal y cita metodológica |
| 01 | **Estructura Gopaldas** | 4 tabs interactivos: Frontend → Métodos → Hallazgos → Backend |
| 02 | **Visualización estadística** | Barras, Boxplot, Línea, Dispersión con overlay técnico + Laboratorio interactivo |
| 03 | **Tarjetas de investigación** | 4 investigaciones aplicadas, una por carrera, con gráficos específicos editables |
| 04 | **Líneas de Investigación IDC** | Las 20 líneas de investigación organizadas por las 4 carreras del IDC |
| 05 | **Footer** | Referencias bibliográficas con DOI verificados |

---

## Paleta de colores corporativa IDC

| Token | Hex | Uso |
|---|---|---|
| Naranja IDC | `#F3A100` | Títulos principales, highlights, valores destacados |
| Azul IDC | `#0072B9` | Subsecciones, botones secundarios, líneas de cota hover |
| Gris Oscuro | `#555553` | Cuerpo de texto explicativo |
| Gris Claro | `#868686` | Metadatos, etiquetas de ejes, detalles secundarios |
| Blanco Técnico | `#FFFFFF` | Trazados técnicos, líneas, flechas, contornos SVG |

---

## Modelo metodológico: Gopaldas (2016)

El panel implementa la estructura de cuatro partes para artículos cualitativos:

```
FRONTEND   →  Problematización, brecha teórica, pregunta de investigación
MÉTODOS    →  Contexto, muestreo teórico, recolección y análisis de datos
HALLAZGOS  →  Secuencia Claim → Data → Elaboration
BACKEND    →  Contribución teórica, implicaciones, extensión de la teoría
```

**Referencia:** Gopaldas, A. (2016). A front-to-back guide to writing a qualitative research article.
*Qualitative Market Research*, 19(1), 115–121. https://doi.org/10.1108/QMR-08-2015-0074

---

## Investigaciones aplicadas incluidas

### Diseño de Interiores
- **Ergonomía y tipografía en espacios comerciales** — Experimento A/B (Serif vs. Sans-serif). Boxplot interactivo de tasa de conversión.

### Diseño Publicitario
- **Predicción de viralidad transmedia** — Regresión múltiple (R²=0.76). Barras de coeficientes β estandarizados editables.

### Diseño de Modas
- **Upcycling y calidad percibida en Lima** — ANOVA 3 grupos (Rústico / Premium / Precio Alto). Gráfico de barras editable.

### Comunicación Audiovisual
- **IA en postproducción cinematográfica** — Experimento cuasiexperimental (Tradicional vs. IA). Boxplot comparativo editable.

---

## Laboratorio interactivo de visualización

El **Laboratorio** (sección 02) permite generar gráficos desde cero ingresando datos propios:

| Gráfico | Campos editables |
|---|---|
| **Barras** | Categorías, valores, título del eje Y |
| **Boxplot** | Mínimo, Q1, Mediana, Q3, Máximo, Outlier |
| **Líneas** | Dos series, valores por período, etiquetas del eje X |
| **Dispersión** | Pares X,Y, coeficiente r, etiquetas de ejes |

### Cómo editar un gráfico

1. Localiza el bloque **EDITOR** dentro de la tarjeta o en el Laboratorio.
2. Modifica los valores en los campos de texto.
3. Presiona **Enter** o haz clic en **↺ Actualizar** para regenerar el gráfico.
4. Si deseas regresar a los datos originales, usa **⟳ Restablecer**.
5. Para guardar el gráfico como archivo, usa **↓ PNG** (imagen rasterizada 3×) o **↓ SVG** (vectorial editable).

> **Nota sobre los formatos de exportación:**
> - **PNG** — resolución 3× (apta para presentaciones, Word, PowerPoint).
> - **SVG** — editable en Adobe Illustrator, Inkscape o Figma; escala sin pérdida.

---

## Líneas de Investigación IDC

### Diseño de Interiores
- Sostenibilidad en el diseño de interiores
- Diseño de interiores para espacios reducidos
- Tecnología y domótica en el diseño de interiores
- Diseño inclusivo y accesible
- Bienestar y ergonomía en espacios comerciales

### Diseño Publicitario
- Estrategias de publicidad digital
- Psicología del color en publicidad
- Publicidad sostenible
- Innovación en publicidad interactiva
- Identidad corporativa y branding

### Diseño de Modas
- Moda sostenible y reciclaje textil
- Innovación textil
- Diseño de moda inclusivo
- Tendencias y consumo responsable
- Tecnología en la moda

### Comunicación Audiovisual
- Narrativas digitales y transmedia
- Cine y documental social
- Innovación en técnicas de postproducción
- Producción audiovisual de bajo presupuesto
- Producción audiovisual en plataformas digitales

---

## Referencias bibliográficas principales

| Referencia | DOI |
|---|---|
| Gopaldas, A. (2016). *QMR* | https://doi.org/10.1108/QMR-08-2015-0074 |
| Vecino-Braña et al. (2022). *PeerJ CS* | https://doi.org/10.7717/peerj-cs.1139 |
| Blanco-Moreno et al. (2024). *JDMM* | https://doi.org/10.1016/j.jdmm.2024.100869 |
| CICIAP (2025). *Boletín BCIV* | https://doi.org/10.60100/bciv.v5i3.270 |
| Cuadernos CDC Palermo (2023) | https://doi.org/10.18682/cdc.vi203.9757 |
| Rivera-Abarca et al. (2025). *Disrupción Metodológica* | https://doi.org/10.56294/dm20251062 |
| Zaldívar-Colado et al. (2024). *RIST* | https://doi.org/10.36867/rist.v58i0.20 |
| Bärtl, M. (2018). *Convergence* | https://doi.org/10.1177/1354856517736979 |
| Cheng et al. (2014). *WWW* | https://doi.org/10.1145/2566486.2567997 |

---

## Requisitos técnicos

| Requisito | Detalle |
|---|---|
| **Navegador** | Chrome 90+, Firefox 88+, Edge 90+, Safari 14+ |
| **Conexión** | Requerida solo para cargar fuentes (Google Fonts / Fontshare) |
| **Servidor** | No requerido — apertura directa como archivo local (`file://`) |
| **Dependencias** | Ninguna instalable — todo via CDN embebido |
| **Tamaño** | ~217 KB (HTML + CSS + JS inline) |

---

## Créditos y autoría

- **Institución:** Instituto de Diseño y Comunicación — IDC
- **Herramienta de generación:** Perplexity AI (asistente de diseño y desarrollo)
- **Metodología de referencia:** Gopaldas (2016) — Qualitative Market Research
- **Versión del archivo:** `index_idc_FINAL.html` — Abril 2026

---

## Historial de versiones

| Versión | Cambios |
|---|---|
| v1.0 | Estructura base: Hero, tabs Gopaldas, sección de gráficos |
| v2.0 | Tarjetas de investigación por carrera con SVG embebidos |
| v3.0 | Laboratorio interactivo con campos de texto editables |
| v4.0 | Editores inline en cada tarjeta de investigación |
| v5.0 | Botones Restablecer + Exportar PNG/SVG + toast de confirmación |
| v5.1 | Corrección diagrama de dispersión (etiqueta r=.82 no superpuesta) |
| v5.2 | Actualización de referencias bibliográficas con DOI verificados |

---

*Documento generado para uso académico y docente — IDC · Lima, Perú · 2026*
