# FORM-TL-01: Taller de Identificacion y Clasificacion de Tipos de Requisitos

Directorio de trabajo y entrega de la actividad formativa **FORM-TL-01**, correspondiente a la Unidad 1 de la asignatura **Ingenieria de Requerimientos (ISR-401)** de la carrera de Ingenieria de Software, Universidad Tecnica Estatal de Quevedo (UTEQ).

---

## Datos Informativos de la Actividad

* **Institucion:** Universidad Tecnica Estatal de Quevedo (UTEQ)
* **Facultad:** Facultad de Ciencias de la Computacion
* **Carrera:** Ingenieria de Software (Rediseno)
* **Asignatura:** Ingenieria de Requerimientos (ISR-401) - 4.o Nivel - Paralelo "A"
* **Unidad Academica:** Unidad 1. Fundamentos de Ingenieria de Requisitos y Proceso de Requisitos
* **Actividad:** FORM-TL-01 - Taller de tipos de requisitos
* **Caracter:** Formativo (sin calificacion; entrega valida es prerrequisito para TA-IND-01 y GA-SUM-01)
* **Modalidad:** Individual
* **Docente:** Prof. Gleiston Ciceron Guerrero Ulloa, PhD (gguerrero@uteq.edu.ec)
* **Estudiante:** Jose Ignacio Gilces Carranza
* **Periodo Academico:** Segundo Periodo Academico Ordinario (SPA) 2026-2027
* **Fecha Limite de Cierre:** Sabado 7 de noviembre de 2026, 23:59
* **Repositorio:** https://github.com/josegilcesc/ISR401-GILCES-JOSE
* **Directorio de la Actividad:** `FORM-TL-01/`

---

## Proposito y Caso de Estudio

* **Proposito:** Ejercitar la distincion formal entre tipos de requisitos (funcionales, de calidad y restricciones; de producto vs. proceso; de sistema vs. software) y la cuantificacion verificable de requisitos de calidad segun las normas ISO/IEC/IEEE 29148:2018 e ISO/IEC 25010:2023.
* **Caso de Estudio:** *Plataforma de gestion de citas medicas - Policlinico Ribera del Quevedo* (centro medico ambulatorio con 24 medicos, 9 especialidades, 18 consultorios y demanda de 450 citas diarias bajo restricciones operativas y normativas de proteccion de datos).

---

## Contenido del Directorio y Entregables

Conforme a la Tabla 1 de la guia de la actividad, este subdirectorio contiene:

```text
FORM-TL-01/
├── README.md                          # Este archivo descriptivo y guia de compilacion
├── main.tex                           # Codigo fuente principal en LaTeX
├── main.pdf                           # Documento compilado y listo para verificacion
├── referencias.bib                    # Fuentes bibliograficas normalizadas en IEEE
```

### Elementos Desarrollados en `main.pdf`:
1. **Clasificacion tridimensional de 20 enunciados (E01 a E20):**
   * *Dimension 1:* Funcional, Calidad (asociando la caracteristica/subcaracteristica de ISO/IEC 25010:2023) o Restriccion.
   * *Dimension 2:* Producto o Proceso.
   * *Dimension 3:* Sistema o Software.
   * *Justificacion tecnica:* Concisa y contextualizada al caso en una sola linea por item.
2. **Cuantificacion de 5 requisitos de calidad vagos:**
   * Reescritura formal de los requisitos no cuantificados del caso ("rapido", "seguro", "facil de usar para adultos mayores", "siempre disponible", "se integre sin problemas") asignando **metrica, unidad de medida y umbral de aceptacion verificable**.
3. **Registro de discrepancias y discusion:**
   * Comparativa de clasificaciones iniciales frente a un companero par, detallando la resolucion tecnica y el argumento normativo acordado.

---

## Reproducibilidad y Compilacion en LaTeX (Criterio P2)

Para regenerar de manera identica y autonoma el documento `main.pdf` a partir del fuente `.tex`:

### 1. Dependencias del Entorno
* **Distribucion:** TeX Live 2024 (o superior), MiKTeX o MacTeX.
* **Compilador primario:** `pdflatex` (version 3.141592653 o superior).
* **Gestor de citas:** `biber` con backend `biblatex`.
* **Paquetes LaTeX requeridos:** `biblatex` (con estilo `ieee`), `booktabs`, `tabularx`, `geometry`, `amsmath`, `hyperref`, `csquotes`, `microtype`.

### 2. Cadena de Comandos de Compilacion
Ejecute la siguiente secuencia en la terminal desde el directorio `FORM-TL-01/`:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

---

## Lista de Cotejo para Autoevaluacion

Previo a la entrega en el SGA, se verifica el cumplimiento de los cinco indicadores de la Tabla 2 de la guia:

* [x] **Indicador 1:** Los 20 enunciados estan clasificados en las tres dimensiones con su debida justificacion.
* [x] **Indicador 2:** Caracteristicas y subcaracteristicas del modelo de calidad ISO/IEC 25010:2023 asignadas con precision.
* [x] **Indicador 3:** Los 5 requisitos de calidad fueron reescritos con metrica, unidad y umbral numerico/verificable.
* [x] **Indicador 4:** Discrepancias registradas y fundamentadas mediante debate entre pares.
* [x] **Indicador 5:** Documento de autoria propia, compilado limpiamente y alojado en el repositorio personal GitHub.

---

## Declaracion de Integridad y Condiciones de Entrega

* **P1 (SGA):** La entrega en el SGA consiste exclusivamente en una caratula de **1 sola pagina** en PDF con datos generales y el enlace directo al repositorio escrito completo en una sola linea.
* **P2 (Reproducibilidad):** El documento se compila sin errores a partir del codigo fuente `.tex`.
* **P3 (Puntualidad):** Todos los commits y artefactos fueron consolidados antes del cierre del sabado 31 de octubre de 2026 a las 23:59.
* **P4 (Integridad y Cero IA no declarada):** Se respetan estrictamente los lineamientos eticos de la ACM y se descarta cualquier indicio grave (G1 a G6). El uso de IA auxiliar queda transparentado con su herramienta, proposito y validacion manual.
