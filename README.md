# Manejo del carcinoma epidermoide cutáneo

Herramienta web de apoyo a la decisión clínica para estadificar el carcinoma
epidermoide cutáneo (CEC) invasivo y obtener las recomendaciones de manejo de las
guías **EADO 2023** (European Association of Dermato‑Oncology, partes 1 y 2),
**AIOM 2024** (Associazione Italiana di Oncologia Medica), **BAD 2020** (British Association
of Dermatologists), **NCCN** (National Comprehensive Cancer Network) y otras guías nacionales,
con la evidencia posterior más relevante. Cada recomendación indica la guía de la que procede.

**Abrir la aplicación:** https://luciamc80.github.io/app-CEC/

## Qué hace

A partir de los datos del caso (edad, inmunodepresión, localización, diámetro
clínico, espesor, diferenciación, subtipo, invasión perineural y ósea, márgenes,
estado ganglionar y metástasis) la aplicación devuelve:

- **TNM y estadio**: AJCC‑8 (American Joint Committee on Cancer) para cabeza y cuello y
  UICC‑8 (Union for International Cancer Control) para tronco y extremidades.
- **Estadio BWH** (Brigham and Women's Hospital) y **riesgo BAD** (bajo, alto, muy alto) con criterios de derivación a comité.
- **Categoría EADO**: bajo riesgo, alto riesgo, localmente avanzado, metástasis
  locorregional o a distancia, con los **factores de alto riesgo** presentes (de los 9 de la guía).
- **Veredictos** de margen quirúrgico, pruebas de imagen, radioterapia postoperatoria
  y tratamiento sistémico.
- Recomendaciones de **cirugía, radioterapia, manejo ganglionar, estudio de extensión,
  tratamiento sistémico, paciente inmunodeprimido, seguimiento y prevención**.
- **Evidencia posterior a las guías** (etiqueta «Post‑guía»): cemiplimab adyuvante (C‑POST, aprobado por la EMA en 2025), KEYNOTE‑630 y novedades de NCCN 2.2026 recogidas en JNCCN 2026 (adyuvancia y neoadyuvancia).
- **Filtro** para ver todas las recomendaciones o solo las de una guía o clasificación
  (EADO, AIOM, AJCC‑8, UICC‑8, BWH, BAD, NCCN, AAD, S3 alemana, SIDeMaST o evidencia posterior).
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
- Keohane SG, et al. British Association of Dermatologists guidelines for cutaneous squamous cell carcinoma 2020. *Br J Dermatol* 2021;184:401–414.
- NCCN Guidelines, Squamous Cell Skin Cancer, versiones 2.2025 y 2.2026.
- Kim JYS, et al. AAD guidelines of care for cutaneous squamous cell carcinoma. *J Am Acad Dermatol* 2018;78:560–578.
- Leiter U, et al. German S3 guideline actinic keratosis and cSCC, update 2023. *EJC Skin Cancer* 2023;1:100004.
- Peris K, et al. Cutaneous squamous cell carcinoma: Italian guidelines by SIDeMaST.
- Las recomendaciones de BAD, NCCN, AAD, S3 alemana y SIDeMaST se recogieron de la revisión comparativa de Paradela de la Morena S, et al. *Actas Dermosifiliogr* 2026;117:104611 y 104612.
- Ma VT. Therapeutic strategies for nonmelanoma skin cancers. *J Natl Compr Canc Netw* 2026;24(Suppl):24–26.
- Evidencia posterior: Rischin D, et al. Adjuvant cemiplimab or placebo in high-risk cutaneous squamous-cell carcinoma (C‑POST). *N Engl J Med* 2025. KEYNOTE‑630: *J Clin Oncol* 2025;43(16 suppl):6000.

## Contenido del repositorio

| Archivo | Descripción |
| --- | --- |
| `index.html` | La aplicación completa (interfaz y lógica en un único archivo). |
| `manifest.webmanifest` | Datos de instalación como app (nombre, iconos, colores). |
| `sw.js` | *Service worker*: permite el uso sin conexión. |
| `fonts/` | Tipografías IBM Plex Sans y JetBrains Mono (licencia SIL Open Font License). |
| `icons/` | Iconos de la app. |
