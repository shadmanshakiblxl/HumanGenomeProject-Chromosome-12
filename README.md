# 🧬 Analysis of Recombination Rates on Human Chromosome 12

> **Linear Regression of Genetic (cM) versus Physical (Mb) Distance in Female Meiosis**  
> **Author:** Shadman Shakib BRAC University Department of Biotechnology  
> **Project:** Human Genome Analysis Series



---

## 📌 Executive Summary

This repository contains an interactive, modern-minimalist web platform presenting research on human meiotic recombination non-uniformity across **Chromosome 12**. 

By applying first-order least-squares linear regression ($y = mx + c$) to digitized positional and genetic map data from female meiosis, this study quantitatively contrasts local recombination rates (cM/Mb) between two distinct chromosomal intervals:

1. **Region A (`Female CEN to 120`)**: Proximal-to-mid chromosome region.
2. **Region B (`Female 120 to End`)**: Distal/telomeric chromosome region.

The findings confirm that physical distance in megabases ($\text{Mb}$) does not scale uniformly with genetic distance in centimorgans ($\text{cM}$), demonstrating localized recombination hotspots and baseline map shifts.

---

## 📊 Key Findings & Mathematical Results

$$\text{Genetic Distance (cM)} = m \cdot \text{Physical Position (Mb)} + c$$

| Sub-Region | Interval Name | Slope ($m$) | Intercept ($c$) | Fitted Equation | Biological Interpretation |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **Region A** | Female CEN to 120 | **`1.40 cM/Mb`** | `-63.69` | $y = 1.40x - 63.69$ | **Higher Recombination Density:** Elevated crossover frequency per physical megabase. |
| **Region B** | Female 120 to End | **`0.95 cM/Mb`** | `-22.64` | $y = 0.95x - 22.64$ | **Lower Recombination Density:** Reduced exchange frequency toward the distal region. |

### 💡 Critical Takeaways
- **+47.4% Rate Variation**: Recombination density in Region A is nearly 1.5 times higher than in Region B.
- **Non-Linear Mapping**: Recombination hotspots create localized steepening along the genetic map, explaining why physical length does not predict genetic distance.

---

## 💻 Web Application Features

The accompanying single-page application (SPA) was built using a **modern minimalist green-scale aesthetic** featuring:

- 🟢 **Interactive Scatter Plot & Linear Regression Canvas**: Switch views dynamically between combined continuous maps and isolated regional datasets with interactive tooltips.
- 📐 **Slope & Rate Calculator**: Allows users to input custom physical coordinates (Mb) to estimate genetic distance (cM) using the fitted linear equations.
- 📜 **Full PDF Paper Viewer**: Embedded research review access with direct link integration.
- 📱 **Fully Responsive Layout**: Built with Tailwind CSS, custom modern typography, and smooth intersection-observer scroll animations.

---

## 🛠️ Tech Stack

- **HTML5 & Modern CSS3** (Custom green tonal palette)
- **Tailwind CSS** (Utility-first UI framework)
- **Chart.js** (Interactive data visualization)
- **Google Fonts** (Inter & JetBrains Mono)
- **Lucide Icons** (Minimal SVG icon set)

---

