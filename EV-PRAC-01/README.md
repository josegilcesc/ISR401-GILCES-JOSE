# EV-PRAC-01 — Evaluación de la Unidad I (Caso «ALERTARÍO»)

Carpeta de entrega y digitalización fiel correspondiente a la evaluación sumativa presencial de la Unidad I de **Ingeniería de Requerimientos (ISR-401)**, Paralelo «B», de la Universidad Técnica Estatal de Quevedo (UTEQ).

## 📌 Datos de la Evaluación

* **Estudiante:** José Ignacio Gilces Carranza
* **Asignatura:** Ingeniería de Requerimientos (ISR-401) — 4.º Nivel, Paralelo «B»
* **Docente:** Prof. Gleiston Cicerón Guerrero Ulloa, PhD
* **Caso de Estudio:** Sistema de Alerta Temprana de Crecidas «ALERTARÍO»
* **Periodo Académico:** SPA 2026–2027

## 📂 Contenido de la Carpeta

```text
EV-PRAC-01/
├── README.md                  # Instrucciones de compilación y descripción de la entrega
├── main.tex                   # Transcripción fiel en LaTeX de la prueba escrita a mano
├── main.pdf                   # Documento PDF compilado reproducible desde main.tex
├── referencias.bib            # Base bibliográfica en formato BibTeX (estilo IEEE/unsrtnat)
├── logoband.png               # Recurso gráfico institucional de la portada (si aplica)
└── evidencias/                # Fotografías originales tomadas en aula antes de entregar
    ├── hoja-01.jpg
    └── hoja-02.jpg
    └── hoja-03.jpg
    └── hoja-04.jpg

```

## ⚙️ Instrucciones de Compilación (Criterio de Piso P2)

Para reproducir el documento `main.pdf` a partir del código fuente `main.tex`:

* **Distribución recomendada:** TeX Live 2024+ o MiKTeX.
* **Compilador:** `pdflatex`
* **Gestor bibliográfico:** `bibtex`
* **Paquetes LaTeX requeridos:** `inputenc`, `fontenc`, `helvet`, `geometry`, `graphicx`, `array`, `tabularx`, `longtable`, `pdflscape`, `colortbl`, `xcolor`, `enumitem`, `fancyhdr`, `lastpage`, `tcolorbox`, `amsmath`, `natbib`, `url`, `needspace`, `caption`, `hyperref`.

### Orden de comandos

Ejecute la siguiente secuencia dentro del directorio `EV-PRAC-01/`:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## ⚖️ Nota de Integridad Académica (Reglas R1–R5)

* El archivo `main.tex` constituye la transcripción fiel de las hojas entregadas en clase.
* Las fotografías originales de las hojas escritas a mano se almacenan exclusivamente en el subdirectorio `evidencias/` y no se incrustan dentro de `main.pdf`.