---
title: "Explicación sobre la arquitectura empresarial"
subtitle: "Basado en el capítulo 3 del libro «Fundamentals of Data Engineering» de Reis y Housley"
author: "Juamini 3 Pro Preview"
date: \today
geometry: margin=1.6in
colorlinks: true
header-includes:
  - \usepackage{fvextra}
  - \DefineVerbatimEnvironment{Highlighting}{Verbatim}{breaklines,commandchars=\\\{\}}
  - \usepackage{graphicx}
	# - \setkeys{Gin}{width=0.95\textwidth}
  - \usepackage{float}
  - \floatplacement{figure}{H}
  - \usepackage{tabularx}
  - \usepackage{array}
  - \renewcommand{\arraystretch}{1.5}
  
  # neutralizamos tightlist y ajustamos espaciado de listas
  - \let\tightlist\relax
  - \usepackage{enumitem}
  - \setlist[itemize,enumerate]{itemsep=1\baselineskip, topsep=1\baselineskip}
  
  # estilo rosado pálido con fuente aclarada
  - \usepackage[most]{tcolorbox}
  - |
    \newtcolorbox{noteBox}{
      colback=red!5!white,
      colframe=red!30!black,
      coltext=black!70,        % color del texto menos saturado
      arc=4pt,
      left=6pt, right=6pt, top=4pt, bottom=4pt,
      boxrule=0.5pt,
      breakable
    }
  - |
    \renewenvironment{quote}{\begin{noteBox}}{\end{noteBox}}

  # --- Caption sin numeración para figuras ---
  - \usepackage{caption}
  - \captionsetup[figure]{labelformat=empty}
---

Para entender esto en el contexto del libro de **Joe Reis y Matt Housley**, hay que salir un poco de la visión puramente técnica y pensar en la organización como un organismo vivo que necesita sobrevivir y adaptarse.

Aquí tienes la explicación desglosada para tu examen:

## 1. ¿Qué es la Arquitectura Empresarial (Enterprise Architecture)?

En el libro, los autores revisan varias definiciones formales (TOGAF, Gartner), pero proponen su propia **definición pragmática**, que es la que deberías saber:

> **"La Arquitectura Empresarial es el diseño de sistemas para soportar el CAMBIO en la empresa, logrado mediante decisiones flexibles y reversibles alcanzadas a través de una evaluación cuidadosa de las compensaciones (trade-offs)."**

**¿Qué significa esto realmente?**
No se trata de hacer diagramas bonitos para colgar en la pared. Se trata de diseñar la estructura de la empresa (tecnología + personas + procesos) para que **no se vuelva rígida** (osificación).

*   El mundo cambia rápido. Si tu arquitectura empresarial es rígida, la empresa muere.
*   Si la arquitectura es buena, la empresa puede pivotar, adoptar nuevas tecnologías o cambiar su modelo de negocio sin colapsar.

## 2. Los Componentes de la Arquitectura Empresarial
Para lograr ese objetivo, la Arquitectura Empresarial funciona como un "paraguas" que cubre cuatro sub-disciplinas. Esto se ve en la **Figura 3-1** del libro:

1.  **Arquitectura de Negocio:** ¿Cuál es la estrategia? ¿Cómo ganamos dinero?
2.  **Arquitectura de Aplicaciones:** ¿Qué software usamos para operar?
3.  **Arquitectura Técnica:** ¿Qué hardware/nube/redes soportan todo?
4.  **Arquitectura de Datos:** (Aquí entras tú). ¿Cómo se mueven y usan los datos?

**Por eso se dice que es un subconjunto:** La Arquitectura de Datos no existe en el vacío; existe para servir a la Arquitectura Empresarial (al negocio).

## 3. El Concepto Clave: Decisiones Reversibles ("Puertas")
Esta es una idea central que Reis toma de Jeff Bezos (Amazon) para explicar una buena arquitectura empresarial:

*   **Puertas de un solo sentido (One-way doors):** Son decisiones casi imposibles de revertir (ej. vender una división de la empresa o elegir una tecnología propietaria que te atrapa por 10 años). Requieren mucho análisis.
*   **Puertas de dos sentidos (Two-way doors):** Son decisiones reversibles. Si te equivocas, puedes volver atrás y corregir (ej. elegir una librería de código abierto estándar).

**El objetivo de la Arquitectura Empresarial según Reis:**
Diseñar el sistema para **maximizar las puertas de dos sentidos**. Queremos poder tomar decisiones rápidas y corregirlas si es necesario, sin que el costo sea catastrófico.

## Resumen para el examen

Si te preguntan qué es la Arquitectura Empresarial y su relación con los datos:

1.  **Definición:** Es el diseño de sistemas enfocado en gestionar y permitir el **cambio** en la organización.
2.  **Relación:** La **Arquitectura de Datos** es un **subconjunto** de ella. Hereda sus propiedades: debe ser flexible, gestionar *trade-offs* y apoyar los objetivos mayores del negocio, no solo los técnicos.
3.  **Meta:** Evitar la rigidez y permitir decisiones reversibles.
