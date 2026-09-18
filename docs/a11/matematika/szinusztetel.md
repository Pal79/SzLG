
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

---

# Szinusztétel

## Háromszög trigonometrikus képlete
A háromszög területe egyenlő két oldal hosszának és az általuk közbezárt szög szinusza szorzatának felével egyenlő.

![trigonometria](../images/matematika-trigonometria-001.svg)

$\frac{a \cdot b \cdot \sin\gamma}{2} = \frac{a \cdot c \cdot \sin\beta}{2} = \frac{b \cdot c \cdot \sin\alpha}{2}$

$$
\begin{aligned}
\frac{a \cdot b \cdot \sin\gamma}{2} = \frac{b \cdot c \cdot \sin\alpha}{2} \quad /\cdot 2  && /\cdot b \\
\frac{a}{c} = \frac{\sin\alpha}{\sin\gamma} \\
\frac{b}{c} = \frac{\sin\beta}{\sin\gamma} \\
\frac{a}{b} = \frac{\sin\alpha}{\sin\beta}
\end{aligned}
$$

A háromszögben két oldal hosszának aránya egyenlő a velük szemközti szögek szinuszának arányával.

---

## Feladatok
$$
\begin{aligned}
a = 3 && \| && \alpha = 30^{\circ} \\
b = ? && \| && \beta = 70^{\circ} \\
c = ? && \| && \gamma = ? \\
\\\\
\gamma = 180^{\circ} - (30^{\circ} + 70^{\circ}) = 80^{\circ} \\
\\\\
b = \frac{b}{a} = \frac{\sin70^{\circ}}{\sin30^{\circ}} \cdot a = \\
\\
= \frac{0.9396}{0.5} \cdot 3 = 1.8792 \cdot 3 = 5.6376 \\
\\\\
c = \frac{c}{a} = \frac{\sin\gamma}{\sin\alpha} \cdot a = \\
\\
= \frac{0.9848}{0.5} \cdot 3 = 1.9696 \cdot 3 = 5.9088
\end{aligned}
$$

---

$$
\begin{aligned}
a = 3 && \| && \alpha = 45^{\circ} \\
b = 4 && \| && \beta = ? \\
c = ? && \| && \gamma = ? \\
\\\\
\beta_{1} = 4 \cdot \frac{\sin\alpha}{3} = 4 \cdot \frac{\sin45^{\circ}}{3} = \frac{0.7071}{3} = 1.2357 \cdot 4 = 70.53^{\circ} \\
\\\\
\gamma = 180^{\circ} - (45^{\circ} + 70.53^{\circ}) = 64.47^{\circ} \\
\\\\
c_{1} = \frac{\sin\gamma}{\sin\alpha} \cdot a = \frac{\sin64.47^{\circ}}{\sin45^{\circ}} \cdot 3 = \frac{0.9023}{0.7071} \cdot 3 = 1.2761 \cdot 3 = 3.8281 \\
\\\\
\\\\
a_{1,2} = 3 \\
b_{1,2} = 4 \\
\alpha = 45^{\circ} \\
\beta_{2} = 180^{\circ} - 70.53^{\circ} = 109.47^{\circ} \\
\gamma_{2} = 25.53^{\circ} \\
\\\\
c_{2} = \frac{\sin\gamma}{\sin\alpha} \cdot a = \frac{\sin25.53^{\circ}}{\sin45^{\circ}} \cdot 3 = \frac{4.4309}{0.7071} \cdot 3 = 6.2662 \cdot 3 = 18.80^{\circ}
\end{aligned}
$$

---

[Vissza](../matematika.md)

---
