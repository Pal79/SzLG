
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

---

[Vissza](./trigonometria.md)

---

# Derékszögű háromszög – összes trigonometriai alak
## Szinusz összes alakja  
$$
\begin{aligned}
\sin(\alpha) &= \frac{\text{szemközti}}{\text{átfogó}} = \frac{a}{c} \\[2em]
\end{aligned}
$$

$$
\begin{array}{|l|l|}
\hline
\text{Keresett} & \text{Képlet} \\
\hline
\text{Szemközti befogó } (a) & a = c \cdot sin(\alpha) \\
\hline
\text{Átfogó } (c) & c = \frac{a}{sin(\alpha)} \\
\hline
\end{array}
$$

## Koszinusz összes alakja  
$$
\begin{aligned}
\cos(\alpha) &= \frac{\text{szomszédos}}{\text{átfogó}} = \frac{b}{c} \\[2em]
\end{aligned}
$$

$$
\begin{array}{|l|l|}
\hline
\text{Keresett} & \text{Képlet} \\
\hline
\text{Szomszédos befogó }(b) & b = c \cdot cos(\alpha) \\
\hline
\text{Átfogó }(c) & c = \frac{b}{cos(\alpha)} \\
\hline
\end{array}
$$

## Tangens összes alakja
$$
\begin{aligned}
\tan(\alpha) &= \frac{\text{szemközti}}{\text{szomszédos}} = \frac{a}{b} \\[2em]
\end{aligned}
$$

$$
\begin{array}{|l|l|}
\hline
\text{Keresett} & \text{Képlet} \\
\hline
\text{Szemközti befogó }(a) & a = b \cdot tan(\alpha) \\
\hline
\text{Szomszédos befogó }(b) & b = \frac{a}{tan(\alpha)} \\
\hline
\end{array}
$$

## Kotangens összes alakja
$$
\begin{aligned}
\cot(\alpha) &= \frac{\text{szomszédos}}{\text{szemközti}} = \frac{b}{a} \\[2em]
\end{aligned}
$$

$$
\begin{array}{|l|l|}
\hline
\text{Keresett} & \text{Képlet} \\
\hline
\text{Szomszédos befogó }(b) & b = a \cdot cot(\alpha) \\
\hline
\text{Szemközti befogó }(a) & a = \frac{b}{cot(\alpha)} \\
\hline
\end{aligned}
$$

# Tetszőleges háromszög – fő tételek
## Szinusztétel
$$
\begin{aligned}
\frac{a}{\sin(\alpha)} &= \frac{b}{\sin(\beta)} = \frac{c}{\sin(\gamma)} \\[2em]
\end{aligned}
$$

$$
\begin{array}{|l|l|}
\hline
\text{Keresett} & \text{Képlet} \\
\hline
\text{Oldal (pl.: a)} & a = \frac{sin(\alpha)}{sin(\beta)} \cdot b \\
\hline
\text{Szög (pl.: }\alpha\text{)} & \alpha = arcsin (\frac{a \cdot sin(\beta)}{b}) \\
\hline
\end{aligned}
$$

## Koszinusztétel
$$
\begin{aligned}
c^{2} &= a^{2} + b^{2} - 2ab \cdot \cos(\gamma) \\[2em]
\end{aligned}
$$

### Oldal keresése  
$$
\begin{aligned}
c &= \sqrt{a^{2} + b^{2} - 2ab \cdot \cos(\gamma)}
\end{aligned}
$$

### Átrendezve szögre:  
$$
\begin{aligned}
\cos(\gamma) &= \frac{a^{2} + b^{2} - c^{2}}{2ab} \\[2em]
\gamma = \cos\left(\frac{a^{2} + b^{2} - c^{2}}{2ab}\right)^{-1} \\[2em]
\end{aligned}
$$

$$
\begin{array}{|l|l|}
\hline
\text{Keresett} & \text{Képlet} \\
\hline
\text{Oldal (pl.: c)} & c = \sqrt{a^{2} + b^{2} - 2ab \cdot cos(\gamma)} \\
\hline
\text{Szög (pl.: }\gamma\text{)} & \gamma = \cos(\frac{a^{2} + b^{2} - c^{2}}{2ab})^{-1} \\
\hline
\end{array}
$$

## Tangens- és kotangens tétel
### Tangens tétel
$$
\begin{aligned}
\frac{a - b}{a + b} &= \frac{\tan\frac{\alpha - \beta}{2}}{\tan\frac{\alpha + \beta}{2}} \\[2em]
\end{aligned}
$$

### Kotangens tétel
$$
\begin{aligned}
\cot(\gamma) = \frac{a^{2} + b^{2} - c^{2}}{4T} \\[2em]
\end{aligned}
$$

# Gyors döntési fa – melyik képletet mikor használod?

$$
begin{array}{|l|l|l|}
\hline
\text{Adott} & \text{Keresett} & \text{Melyik tétel?} \\
\hline
\text{Derékszög + szög + oldal} & \text{Másik oldal} & \sin | \cos | \tan | \cot \\
\hline
\text{Derékszög + két oldal} & \text{Szög} & \tan^{-1} | \sin{-1} | \cos^{-1} \\
\hline
\text{Két oldal + közbezárt szög} & \text{Harmadik oldal} & \text{Koszinusztétel} \\
\hline
\text{Három oldal} & \text{Bármelyik szög} & \text{Koszinusztétel (szögre rendezvve)} \\
\hline
\text{Két szög + egy oldal} & \text{Másik oldal} & \text{Szinusztétel} \\
\hline
\text{Egy oldal + két szög} & \text{Harmadik szög} & 180^{\circ} - (\alpha + \beta) \\
\hline
\text{Két oldal + nem közbezárt szög} & \text{Oldal vagy szög} & \text{Szinusztétel} \\
\hline
\end{array}
$$

---

[Vissza](./trigonometria.md)

---
