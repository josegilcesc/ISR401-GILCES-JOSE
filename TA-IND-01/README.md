# Trabajo Autónomo Individual: TA-IND-01
**Asignatura:** Ingeniería de Requerimientos (ISR-401)  
**Institución:** Universidad Técnica Estatal de Quevedo (UTEQ) - Facultad de Ciencias de la Computación  
**Periodo Académico:** Segundo Periodo Académico Ordinario (SPA) 2026-2027  
**Estudiante:** José Ignacio Gilces Carranza  
**Docente:** Gleiston Cicerón Guerrero Ulloa, PhD  

---

## 📋 Descripción General del Repositorio
Este directorio `TA-IND-01` contiene el desarrollo integral del **Trabajo Autónomo Individual TA-IND-01**, enfocado en la aplicación rigurosa de la norma internacional **ISO/IEC/IEEE 29148:2018** y el modelo de calidad de producto **ISO/IEC 25010:2023** sobre un sistema de software real en producción: el **Sistema de Gestión Académica (SGA)** de la UTEQ.

El informe cumple estrictamente con los lineamientos del Encuadre Académico de la asignatura, integrando un resumen analítico, un glosario técnico, especificaciones formales de requisitos bajo sintaxis imperativa estricta, autoevaluación frente a términos prohibidos, y una reflexión crítica fundamentada.

---

## 📂 Estructura de Archivos del Repositorio
Para garantizar la **reproducibilidad** del entregable (Criterio de piso P2 del Encuadre), el repositorio contiene los siguientes recursos fuente:

* `main.tex`: Código fuente principal del informe redactado en $\LaTeX$.
* `main.pdf`: Documento final compilado (informe completo de 7 páginas).
* `README.md`: Este archivo de documentación técnica del repositorio.

---

## 🛠️ Instrucciones de Compilación (Reproducibilidad)
El informe se encuentra escrito en $\LaTeX$ estándar. Para clonar el repositorio y regenerar el archivo `main.pdf` de forma idéntica, ejecute la siguiente secuencia de comandos en su terminal:

```bash
# 1. Clonar el repositorio
git clone https://github.com/josegilcesc/ISR401-GILCES-JOSE.git
cd ISR401-GILCES-JOSE/TA-IND-01

# 2. Secuencia de compilación recomendada (compatible con pdflatex y biber)
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

### ⚙️ Dependencias y Entorno de Compilación
* **Compilador LaTeX:** `pdfTeX` (versión 3.141592653 o superior).
* **Gestor de Bibliografía:** `biber` (para referencias en formato IEEE conforme al estándar exigido).
* **Clases y Paquetes principales:** `IEEEtran`, `tabularx`, `amsmath`, `biblatex`.

---

## 🔍 Resumen del Contenido del Informe
1. **Descripción del Sistema:** Análisis contextual, propósito, usuarios y arquitectura del SGA UTEQ (concurrencia de hasta 2500 usuarios activos).
2. **Resumen Analítico (ISO/IEC/IEEE 29148:2018):** Estudio de las cláusulas 5.2.4 (estructura imperativa con *shall*), 5.2.5 (características individuales), 5.2.6 (coherencia de conjunto) y 5.2.7 (términos vagos prohibidos).
3. **Glosario Técnico:** Diez términos contextualizados de la cláusula 3 de la norma aplicados directamente al dominio del SGA.
4. **Especificación Formal de Requisitos:** Quince requisitos (funcionales, de interfaz, restricciones e ISO/IEC 25010:2023 cuantificados mediante percentiles y métricas de laboratorio).
5. **Matriz de Clasificación y Autoevaluación:** Corrección rigurosa de enunciados ambiguos eliminando adjetivos subjetivos ("rápido", "fácil", "amigable", "seguro").
6. **Reflexión Crítica y Conclusiones.**
7. **Declaración de Uso de IA:** Transparencia académica conforme a las políticas del curso.
