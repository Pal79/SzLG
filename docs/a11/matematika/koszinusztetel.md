
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

---

[Vissza](./szogfuggvenyek.md)

---

# Koszinusztétel
Egy háromszög egyik oldalhosszának négyzetét megkaphatjuk, ha a másik két oldal hossza négyzetének összegéből kivonjuk a két oldal hosszának és a közbezárt szög koszinuszának kétszeres szorzatát.

A **koszinusztétel** a pitagoraszi tétel általánosítása tetszőleges (nem csak derékszögű) háromszögekre.

## Tétel képlete
Bármely háromszögben, ahol a háromszög oldalai `a`, `b` és `c`, a velük szemközti szögek pedig rendre $\alpha$, $\beta$ és $\gamma$:

$$
\begin{aligned}
c^{2} &= a^{2} + b^{2} - 2ab \cdot \cos\gamma
\end{aligned}
$$

Ugyanígy felírható a többi oldalra is:

$$
\begin{aligned}
a^{2} &= b^{2} + c^{2} - 2bc \cdot \cos\alpha \\[1em]
b^{2} &= a^{2} + c^{2} - 2ac \cdot \cos\beta
\end{aligned}
$$

A koszinusztételt akkor alkalmazzuk, ha a háromszögben ismerjük:
- **Két oldalt és a közbezárt szögüket** (így kiszámítható a harmadik oldal).
- **Mindhárom oldalt** (így kiszámítható bármelyik szög).

## Szög kiszámítása az oldalakból
A képlet átrendezésével bármelyik szög koszinusza kifejezhető. Például a $\gamma$ szögre:

$$
\begin{aligned}
\cos\gamma &= \frac{a^{2} + b^{2} - c^{2}}{2ab}
\end{aligned}
$$

Ha a közbezárt szög derékszög ($\gamma = 90^{\circ}$), akkor $\cos(90^{\circ}) = 0$, így a tétel pontosan a **Pitagorasz-tétel**t adja vissza ($c^{2} = a^{2} + b^{2}$)

## 3320. Feladat

$$
\begin{array}{|c|c|c|c|c|c|c|}
\hline
& a & b & c & \alpha & \beta & \gamma \\
\hline
\text{1.sor} & 9\text{ cm} & 8\text{ cm} & & & & 70^{\circ} \\
\hline
\text{2.sor} & & 12.4\text{ m} & 8.3\text{ m} & 110^{\circ} & & \\
\hline
\text{3.sor} & 18\text{ dm} & & 120\text{ cm} & & 69^{\circ} & \\
\hline
\end{array}
$$

### 1.sor
$$
\begin{array}{|l|l|}
a = 9\text{ cm} & \alpha = \text{?} \\
b = 8\text{ cm} & \beta = \text{?} \\
c = \text{?} & \gamma = 70^{\circ} \\
\end{array}
$$
$$
\begin{aligned}
\\[2em]
c^{2} &= a^{2} + b^{2} - 2ab \cdot \cos\gamma = 9^{2} + 8^{2} - 2 \cdot 9 \cdot 8 \cdot \cos70^{\circ} = 145 - 144 \cdot 0.342 = 95.752 \\[.5em]
c &= \sqrt{95.752} = 9.79cm \\[1em]
\sin\alpha &= \frac{\sin\gamma}{c} \cdot a = \frac{\sin70^{\circ}}{9.79} \cdot 9 = \frac{0.9397}{9.79} \cdot 9 = 0.096 \cdot 9 = 0.864 \\[.5em]
\alpha &= \sin^{-1}(0.864) = 59.77^{\circ} \\[1em]
\beta &= 180^{\circ} - (59.77^{\circ} + 70^{\circ}) = 50.23^{\circ}
\end{aligned}
$$

### 2.sor
$$
\begin{array}{|l|l|}
a = \text{?} & \alpha = 110^{\circ} \\
b = 12.4\text{ m} & \beta = \text{?} \\
c = 8.3\text{ m} & \gamma = \text{?} \\
\end{array}
$$
$$
\begin{aligned}
\\[2em]
a^{2} &= b^{2} + c^{2} - 2bc \cdot \cos\alpha = 12.4^{\circ} + 8.3^{2} - 2 \cdot 12.4 \cdot 8.3 \cdot \cos110^{\circ} = 222.65 - 205.84 \cdot (-0.342) = 293 \\[.5em]
a &= \sqrt{293} = 17.12m \\[1em]
\sin\beta &= \frac{\sin\alpha}{a} \cdot b = \frac{\sin110^{\circ}}{17.12} \cdot 12.4 = 0.055 \cdot 12.4 = 0.682 \\[.5em]
\beta &= \sin^{-1}(0.682) = 43^{\circ} \\[1em]
\gamma &= 180^{\circ} - (43^{\circ} + 110^{\circ}) = 27^{\circ}
\end{aligned}
$$

### 3.sor
$$
\begin{array}{|l|l|}
a = 18\text{ dm} & \alpha = \text{?} \\
b = \text{?} & \beta = 69^{\circ} \\
c = 120\text{ cm} = 12\text{ dm} & \gamma = \text{?} \\
\end{array}
$$
$$
\begin{aligned}
\\[2em]
b^{2} &= a^{2} + c^{2} - 2ac \cdot \cos\beta = 18^{2} + 12^{2} - 2 \cdot 18 \cdot 12 \cdot \cos69^{\circ} = 468 - 432 \cdot 0.3583 = 468 - 154.79 = 313.21 \\[.5em]
b &= \sqrt{313.21} = 17.7dm \\[1em]
\sin\alpha &= \frac{\sin\beta}{b} \cdot a = \frac{\sin69^{\circ}}{17.7} \cdot 18 = \frac{0.9336}{17.7} \cdot 18 = 0.0527 \cdot 18 = 0.9468 \\[.5em]
\alpha &= \sin{-1}(0.9486) = 71.55^{\circ} \\[1em]
\gamma &= 180^{\circ} - (71.55^{\circ} + 69^{\circ}) = 39.45^{\circ}
\end{aligned}
$$

### Megoldás

$$
\begin{array}{\|c\|c\|c\|c\|c\|c\|c\|}
\hline
& a & b & c & \alpha & \beta & \gamma \\
\hline
\text{1. sor} & 9\text{ cm} & 8\text{ cm} & 9.79\text{ cm} & 59.77^\circ & 50.23^\circ & 70^\circ \\
\hline
\text{2. sor} & 17.12\text{ m} & 12.4\text{ m} & 8.3\text{ m} & 110^\circ & 43^\circ & 27^\circ \\
\hline
\text{3. sor} & 18\text{ dm} & 17.7\text{ dm} & 120\text{ cm} & 71.55^\circ & 69^\circ & 39.45^\circ \\
\hline
\end{array}
$$

---

$$
\begin{array}{|l|l|}
a = 10\text{ cm} & \alpha = \text{?} \\
b = 6\text{ cm} & \beta = 30^{\circ} \\
c = \text{?} & \gamma = \text{?}
\end{array}
$$
$$
\begin{aligned}
\\[1em]
\frac{\sin\alpha}{a} &= \frac{\sin\beta}{b} = \frac{\sin\alpha}{10} = \frac{\sin30^{\circ}}{6} \quad / \cdot 10 \\
\sin\alpha &= \frac{10 \cdot \sin30^{\circ}}{6} = 0.833 \\
\alpha &= \sin^{-1}(0.833) = 56.41^{\circ} \\[1em]
\gamma &= 180^{\circ} - (56.41^{\circ} + 30^{\circ}) = 93.59^{\circ} \\[1em]
c^{2} &= a^{2} + b^{2} - 2ab \cdot \cos\gamma = 10^{2} + 6^{2} - 2 \cdot 10 \cdot 6 \cdot \cos93.59^{\circ} = 136 - 120 \cdot (-0.0626) = 136 - (-7.512) = 143.512 \\
c &= \sqrt{143.512} = 11.98\text{ cm}
\end{aligned}
$$

---

$$
\begin{array}{|l|l|}
a = 10 & \alpha = \text{?} \\
b = 15 & \beta = \text{?} \\
c = \text{?} & \gamma = 60^{\circ}
\end{array}
$$
$$
\begin{aligned}
c^{2} &= a^{2} + b^{2} - 2ab \cdot \cos\gamma = 10^{2} + 15^{2} - 2 \cdot 10 \cdot 15 \cdot \cos60^{\circ} = 325 - 300 \cdot 0.5 = 325 - 150 = 175 \\
c &= \sqrt{175} = 13.23 \\[1em]
\frac{\sin\alpha}{a} &= \frac{\sin\gamma}{c} = \frac{\sin\alpha}{10} = \frac{\sin60^{\circ}}{13.23} \\
\sin\alpha &= \frac{10 \cdot \sin60^{\circ}}{13.23} = \frac{8.66}{13.23} = 0.655 \\
\alpha &= \sin^{-1}(0.655) = 40.92^{\circ} \\[1em]
\beta &= 180^{\circ} - (40.92^{\circ} + 60^{\circ}) = 79.08^{\circ}
\end{aligned}
$$

---

[Vissza](./szogfuggvenyek.md)

---
