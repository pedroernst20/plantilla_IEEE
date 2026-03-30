# 📑 Plantilla de Informes IEEE - UTN FRC

![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-the-badge&logo=latex&logoColor=white)
![Engineering](https://img.shields.io/badge/Ingeniería-Electrónica-blue?style=for-the-badge)
![University](https://img.shields.io/badge/UTN-FRC-red?style=for-the-badge)

Esta es una plantilla personalizada de LaTeX (`.cls`) diseñada específicamente para estudiantes de **Ingeniería Electrónica** en la **UTN - Facultad Regional Córdoba**. Transforma el formato estándar de informes en un documento profesional bajo las normas **IEEE**, optimizado para entregas de cátedra.

---

## 🚀 Características Principales

- **Formato IEEE Estricto:** Cumple con la diagramación de doble columna, tipografía Times New Roman y jerarquía de títulos.
- **Encabezado Automatizado:** Título en 24pt, autores en 11pt (negrita cursiva) y afiliación institucional en 10pt (cursiva) según requerimientos específicos.
- **Comandos de Unidades:** Incluye atajos para magnitudes eléctricas comunes ($\Omega$, $\kohm$, $\uF$, $\V$, $\mA$, etc.) para agilizar la escritura de cálculos.
- **Soporte para Circuitos:** Configurado para trabajar nativamente con `circuitikz` y `pgfplots`, ideal para diagramas electrónicos y gráficos de señales.

---

## 📁 Estructura del Repositorio

| Archivo | Descripción |
| :--- | :--- |
| `plantilla.cls` | El motor de la plantilla. Contiene todas las definiciones de estilo y comandos. |
| `ejemplo.tex` | Archivo de ejemplo con la estructura básica para empezar a escribir. |
| `ejemplo.pdf` | **Previsualización del resultado final** para ver el layout y las fuentes. |

---

## 🛠️ Cómo empezar

1. Descargá `plantilla.cls` y ponelo en la misma carpeta que tu proyecto de LaTeX (o subilo a Overleaf).
2. En tu archivo `.tex` principal, configurá el preámbulo de la siguiente manera:

```latex
\documentclass{plantilla}

% Datos del informe
\materia{Sistemas de Comunicación}
\comision{4R2}
\titulo{Título del Informe \\ con Salto de Línea}
\autores{Pedro Ernst, Valentino Rao}

\begin{document}
\maketitle

\begin{abstract}
Tu resumen aquí...
\end{abstract}

\section{Introducción}
\IEEEPARSTART{E}{ste} es el comienzo de un gran informe...
