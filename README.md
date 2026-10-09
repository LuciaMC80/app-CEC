# Manejo del carcinoma epidermoide cutáneo

Herramienta web de apoyo a la decisión clínica para estadificar el carcinoma
epidermoide cutáneo (CEC) invasivo y obtener las recomendaciones de manejo de las
guías **EADO 2023** (partes 1 y 2) y **AIOM 2024**. Cada recomendación indica la
guía de la que procede y su grado.

**Abrir la aplicación:** https://luciamc80.github.io/app-CEC/

## Qué hace

A partir de los datos del caso (edad, inmunodepresión, localización, diámetro
clínico, espesor, diferenciación, subtipo, invasión perineural y ósea, márgenes,
estado ganglionar y metástasis) la aplicación devuelve:

- **TNM y estadio**: AJCC 8.ª edición para cabeza y cuello y UICC 8.ª edición para
  tronco y extremidades.
- **Estadio BWH** (Brigham and Women's Hospital).
- **Categoría EADO**: bajo riesgo, alto riesgo, localmente avanzado, metástasis
  locorregional o a distancia, con los **factores de alto riesgo** presentes (de los 9 de la guía).
- **Veredictos** de margen quirúrgico, pruebas de imagen, radioterapia postoperatoria
  y tratamiento sistémico.
- Recomendaciones de **cirugía, radioterapia, manejo ganglionar, estudio de extensión,
  tratamiento sistémico, paciente inmunodeprimido, seguimiento y prevención**.
- **Evidencia posterior a las guías** (etiqueta «Post‑guía»): cemiplimab adyuvante (C‑POST, aprobado por la EMA en 2025) y KEYNOTE‑630.
- Filtro para ver las recomendaciones de **una sola guía** o solo la evidencia posterior.
- **Resumen imprimible** del caso.

## Uso en el móvil

Se abre desde el navegador con el enlace de arriba. Para dejarla como una app:

- **Android (Chrome):** menú ⋮ → *Añadir a pantalla de inicio*.
- **iPhone (Safari):** botón de compartir → *Añadir a pantalla de inicio*.

Instalada de este modo funciona **sin conexión**: el contenido se guarda en el
dispositivo la primera vez que se abre.

## Compartir un caso

El botón **Compartir caso** genera un enlace que lleva los datos del caso en la
propia dirección (después de `#`). Al abrirlo, la aplicación reproduce el caso tal
cual. En el móvil se abre directamente el menú de compartir del sistema.

Los datos del caso **no salen del dispositivo**: viajan dentro del enlace y solo
llegan a quien se lo envíe. La aplicación no tiene servidor, no guarda nada y no
registra ninguna información.

## Aviso

Herramienta de apoyo a la decisión. **No sustituye el juicio clínico ni la
valoración del comité multidisciplinar de tumores.** No es un producto sanitario
certificado y no debe usarse como única base de una decisión asistencial. Sólo para
CEC invasivo: excluye la enfermedad de Bowen y los carcinomas epidermoides mucosos.

## Fuentes

- Stratigos AJ, et al. European consensus-based interdisciplinary guideline for invasive
  cutaneous squamous cell carcinoma. Part 1: Diagnostics and prevention — Update 2023.
  *Eur J Cancer* 2023;193:113251.
- Stratigos AJ, et al. European consensus-based interdisciplinary guideline for invasive
  cutaneous squamous cell carcinoma. Part 2: Treatment — Update 2023.
  *Eur J Cancer* 2023;193:113252.
- Queirolo P, et al. Guidelines for the diagnosis and treatment of cutaneous squamous cell
  carcinoma: a GRADE approach for evidence evaluation and recommendations by the Italian
  Association of Medical Oncology. *ESMO Open* 2024;9(5):103005.
- AJCC Cancer Staging Manual, 8.ª edición. UICC TNM Classification of Malignant Tumours, 8.ª edición.
- Evidencia posterior: Rischin D, et al. Adjuvant cemiplimab or placebo in high-risk cutaneous squamous-cell carcinoma (C‑POST). *N Engl J Med* 2025. KEYNOTE‑630: *J Clin Oncol* 2025;43(16 suppl):6000.

## Contenido del repositorio

| Archivo | Descripción |
| --- | --- |
| `index.html` | La aplicación completa (interfaz y lógica en un único archivo). |
| `manifest.webmanifest` | Datos de instalación como app (nombre, iconos, colores). |
| `sw.js` | *Service worker*: permite el uso sin conexión. |
| `fonts/` | Tipografías IBM Plex Sans y JetBrains Mono (licencia SIL Open Font License). |
| `icons/` | Iconos de la app. |
