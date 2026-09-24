#Analysis of Recombination Rates on Human Chromosome 12

> **Linear Regression of Genetic (cM) versus Physical (Mb) Distance in Female Meiosis**  
> **Author:** Shadman Shakib BRAC University Department of Biotechnology  
> **Project:** Human Genome Analysis Series



---

##  Executive Summary

This repository contains an interactive, modern-minimalist web platform presenting research on human meiotic recombination non-uniformity across **Chromosome 12**. 

By applying first-order least-squares linear regression ($y = mx + c$) to digitized positional and genetic map data from female meiosis, this study quantitatively contrasts local recombination rates (cM/Mb) between two distinct chromosomal intervals:

1. **Region A (`Female CEN to 120`)**: Proximal-to-mid chromosome region.
2. **Region B (`Female 120 to End`)**: Distal/telomeric chromosome region.

The findings confirm that physical distance in megabases ($\text{Mb}$) does not scale uniformly with genetic distance in centimorgans ($\text{cM}$), demonstrating localized recombination hotspots and baseline map shifts.

---

# Human Chromosome 12 Recombination Rate Analysis

This repository contains the dataset, linear regression scripts, and analytical findings for the female meiotic recombination rate analysis on **Human Chromosome 12**. The study compares genetic distance ($\text{cM}$) against physical distance ($\text{Mb}$) to demonstrate the non-uniformity of recombination rates across genomic regions.

---



* **Primary Objective:** Quantify regional meiotic recombination rates ($\text{cM/Mb}$) along the $q$-arm of female Chromosome 12 using Ordinary Least-Squares (OLS) linear regression ($y = mx + c$).



---

##  Key Findings

* **Region A (Female CEN to 120):**
* **Equation:** $y = 0.99x - 32.33$ ($R^2 \approx 0.986$)


* **Recombination Rate:** $0.99 \text{ cM/Mb}$



* **Region B (Female 120 to End):**
* **Equation:** $y = 1.45x - 79.71$ ($R^2 \approx 0.984$)


* **Recombination Rate:** $1.45 \text{ cM/Mb}$



* **Rate Shift:** Transitioning from the proximal pericentromeric region (Region A) to the distal telomeric region (Region B) yields a **46.46% increase** in recombination rate:



$$\frac{1.45 - 0.99}{0.99} \times 100\% \approx 46.46\%$$




---

## Dataset Summary

Data coordinates were digitized from high-resolution genetic maps using computer-assisted image software (WebPlotDigitizer).

| Metric | Region A (Female CEN to 120) | Region B (Female 120 to End) |
| --- | --- | --- |
| **Data Points** | 19 coordinate pairs

 | 18 coordinate pairs

 |
| **Physical Range (Mb)** | $40.07 - 110.14 \text{ Mb}$<br> | $106.30 - 150.73 \text{ Mb}$<br> |
| **Genetic Range (cM)** | $2.99 - 78.10 \text{ cM}$<br> | $74.51 - 139.01 \text{ cM}$<br> |
| **Slope ($m$)** | $0.99 \text{ cM/Mb}$<br> | $1.45 \text{ cM/Mb}$<br> |
| **Intercept ($c$)** | $-32.33$<br> | $-79.71$<br> |



##  Usage

### Prerequisites

Ensure Python 3.x is installed along with the required libraries:

```bash
pip install numpy pandas matplotlib scipy

```

### Running the Analysis

Execute the main regression script to calculate slope parameters and produce visualization plots:

```bash
python scripts/regression_analysis.py

```

---

##  Biological Context & Discussion

1. **Decoupling of Distances:** The physical genome ($\text{Mb}$) does not linearly map to genetic recombination ($\text{cM}$).


2. **Telomeric Enhancement:** Higher crossover frequencies occur in the distal telomeric region (Region B) compared to the pericentromeric region (Region A).


3. **Hotspots & Chromatin Architecture:** Local fluctuations in slope illustrate the impact of regional chromatin structure and recombination hotspots across female meiosis.



---

##  References

* **International Human Genome Sequencing Consortium** (2001). Initial sequencing and analysis of the human genome. *Nature*, 409(6822), 860–921.


* **Kong, A., et al.** (2002). A high-resolution recombination map of the human genome. *Nature Genetics*, 31(3), 241–247.


* **Myers, S., et al.** (2005). A fine-scale map of recombination rates and hotspots across the human genome. *Science*, 310(5746), 321–324.


* **Yu, A., et al.** (2001). Comparison of human genetic and sequence-based physical maps. *Nature*, 409(6822), 951–953.



## Web Application Features

The accompanying single-page application (SPA) was built using a **modern minimalist green-scale aesthetic** featuring:

-  **Interactive Scatter Plot & Linear Regression Canvas**: Switch views dynamically between combined continuous maps and isolated regional datasets with interactive tooltips.
-  **Slope & Rate Calculator**: Allows users to input custom physical coordinates (Mb) to estimate genetic distance (cM) using the fitted linear equations.
- **Full PDF Paper Viewer**: Embedded research review access with direct link integration.
- **Fully Responsive Layout**: Built with Tailwind CSS, custom modern typography, and smooth intersection-observer scroll animations.

---

## 🛠️ Tech Stack

- **HTML5 & Modern CSS3** (Custom green tonal palette)
- **Tailwind CSS** (Utility-first UI framework)
- **Chart.js** (Interactive data visualization)
- **Google Fonts** (Inter & JetBrains Mono)
- **Lucide Icons** (Minimal SVG icon set)

---

