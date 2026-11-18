# ISR401 — Ingeniería de Requerimientos

Repositorio académico individual para el desarrollo, control de versiones y entrega de actividades formativas, sumativas y artefactos de la asignatura **Ingeniería de Requerimientos (ISR-401)**, correspondiente a la carrera de Software de la Universidad Técnica Estatal de Quevedo (UTEQ).

---

## 📌 Datos Informativos

* **Institución:** Universidad Técnica Estatal de Quevedo (UTEQ)
* **Facultad:** Facultad de Ciencias de la Computación
* **Carrera:** Ingeniería de Software (Rediseño)
* **Asignatura:** Ingeniería de Requerimientos (ISR-401)
* **Nivel / Paralelo:** 4.º Nivel — Paralelo «A»
* **Periodo Académico:** Segundo Periodo Académico Ordinario (SPA) 2026–2027
* **Docente:** Prof. Gleiston Cicerón Guerrero Ulloa, PhD (gguerrero@uteq.edu.ec)
* **Estudiante:** José Gilces
* **URL del Repositorio:** https://github.com/josegilcesc/ISR401-GILCES-JOSE

---

## 📂 Estructura del Repositorio

El contenido evaluable se organiza de acuerdo con los componentes del sistema de evaluación del encuadre (Gestión de Aula, Trabajo Autónomo y Evaluaciones):

```text
ISR401-GILCES-JOSE/
├── README.md                          # Documentación e instrucciones de reproducción
├── .gitignore                         # Exclusión de binarios temporales y auxiliares de LaTeX
│
├── 01_Trabajo_Autonomo/               # Componente TA
│   ├── TA-IND-01/                     # IEEE 29148 y tipos de requisitos
│   ├── TA-IND-02/                     # Priorización (MoSCoW, Kano, ponderada)
│   ├── TA-IND-03/                     # Modelos de datos, función y comportamiento
│   └── TA-IND-04/                     # Matriz de trazabilidad y análisis de impacto
│
├── 02_Practicas_Experimentales/       # Componente GA (PE-U)
│   ├── GA-SUM-01_PE-U1/               # Proceso de requisitos y framework IR
│   ├── GA-SUM-03_PE-U2/               # Elicitación y análisis
│   ├── GA-SUM-04_PE-U3/               # Especificación de requisitos (ERS)
│   ├── GA-SUM-05_PE-U4/               # Validación y aseguramiento de calidad
│   └── GA-SUM-07_PE-U5/               # IR ágil aplicada
│
├── 03_Proyecto_Fin_de_Curso/          # Entregas del PFC (TA-PFC)
│   ├── TA-PFC-E1/                     # Entrega 1: Visión, alcance y plan de elicitación
│   ├── TA-PFC-E2/                     # Entrega 2: Evidencias de campo, análisis y casos de uso
│   ├── TA-PFC-E3/                     # Entrega 3: ERS (IEEE 29148), UML e inspección
│   └── TA-PFC-E4/                     # Entrega final: ERS validado, backlog y métricas
│
└── 04_Evaluaciones/                   # Componente EV (Casos prácticos de exámenes)
    ├── EV-SUM-01_U1/
    ├── EV-SUM-02_U2/
    ├── EV-SUM-03_U3/
    ├── EV-SUM-04_U4/
    └── EV-SUM-05_U5/
```

> **Nota:** Cada subdirectorio de actividad contiene sus respectivos archivos fuente `.tex`, archivo de bibliografía `.bib`, carpeta `figures/` o `evidencias/` (cuando aplique) y el documento final compilado `.pdf`.

---

## ⚙️ Reproducibilidad y Compilación en LaTeX

Conforme a la norma de entrega y al **Criterio de Piso P2**, todo informe debe poder regenerarse fielmente clonando el repositorio y ejecutando la compilación.

### Entorno y Dependencias Requeridas
* **Distribución recomendada:** TeX Live 2024+, MiKTeX o MacTeX.
* **Compilador del documento:** `pdflatex` (o `xelatex` según se especifique en la plantilla).
* **Gestor bibliográfico:** `biber` (con backend `biblatex`).
* **Paquetes clave:** `biblatex` (estilo `ieee`), `geometry`, `graphicx`, `booktabs`, `hyperref`, `amsmath`, `microtype`, `csquotes`.

### Secuencia de Compilación Estándar
Para garantizar la resolución correcta de hipervínculos, índices y citas bibliográficas en estilo IEEE, se debe ejecutar la siguiente cadena de comandos desde la carpeta de la actividad:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

---

## 📚 Estándar de Referencias Bibliográficas

* Todas las citas y fuentes consultadas siguen estrictamente la norma **IEEE** gestionadas con **`biblatex`**.
* Conforme al **Criterio de Piso P4** y la dimensión **D6**, todas las referencias listadas corresponden a obras reales, verificables y vigentes, con sus respectivos autores, año, título, editorial/revista y código DOI/ISBN verificado.
* **Bibliografía base de la materia:**
  * ISO/IEC/IEEE 29148:2018 — *Requirements Engineering*.
  * Klaus Pohl (2025) — *Requirements Engineering: Fundamentals, Principles, and Techniques* (2.ª ed.).
  * IEEE Computer Society (2024) — *Guide to the SWEBOK v4.0*.
  * ISO/IEC 25010:2023 — *Product Quality Model*.

---

## ⚖️ Declaración de Integridad Académica y Uso de IA

Este repositorio opera bajo el **Código de Ética de la ACM** y las políticas de integridad académica del Encuadre:

1. **Autoría propia:** Todo contenido técnico, modelado, redacción y evidencias de campo corresponden a la autoría y análisis del estudiante o del equipo de trabajo.
2. **Uso ético y declarado de IA:** La inteligencia artificial generativa no sustituye el trabajo que se evalúa. Cualquier empleo de herramientas como apoyo auxiliar (por ejemplo, depuración de errores de compilación de LaTeX o revisión ortográfica) se detalla de forma explícita en cada informe entregado indicando: *herramienta, versión, propósito exacto y método de verificación manual aplicado*.
3. **Control de indicios de IA:** Se mantiene estricta rigurosidad para descartar referencias artificiales, citas sin respaldo, alucinaciones o textos genéricos desvinculados del caso de estudio real.

---

## ⏱️ Política de Commits y Trabajo Anticipado

En cumplimiento de la Sección 6 y la rúbrica de desempeño:
* Las entregas cierran los **sábados a las 23:59** de la semana correspondiente a la actividad.
* El historial de control de versiones en Git refleja **trabajo sustantivo y distribuido en al menos tres días distintos** a lo largo del plazo, evitando concentrar más del 50 % de las modificaciones dentro de las últimas 24 horas previas al cierre para prevenir penalizaciones en la calificación y en el aporte individual.
