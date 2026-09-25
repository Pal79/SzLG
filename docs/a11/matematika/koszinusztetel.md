
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

---

[Vissza](../matematika.md)

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

### Szög kiszámítása az oldalakból
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
\text{2.sor} & & 12.4\text{ m} & 8.3\text{ m} & 110^{\circ} & & \\
\text{3.sor} & 18\text{ dm} & & 120\text{ cm} & & 69^{\circ} & \\
\hline
\end{array}
$$

### 1.sor
$$
\begin{aligned}
a &= 9cm &&|&& \alpha = ? \\
b &= 8cm &&|&& \beta = ? \\
c &= ? &&|&& \gamma = 70^{\circ} \\[1em]
c^{2} &= a^{2} + b^{2} - 2ab \cdot \cos\gamma = 9^{2} + 8^{2} - 2 \cdot 9 \cdot 8 \cdot \cos70^{\circ} = 145 - 144 \cdot 0.342 = 95.752 \\[.5em]
c &= \sqrt{95.752} = 9.79cm \\[1em]
\sin\alpha &= \frac{\sin\gamma}{c} \cdot a = \frac{\sin70^{\circ}}{9.79} \cdot 9 = \frac{0.9397}{9.79} \cdot 9 = 0.096 \cdot 9 = 0.864 \\[.5em]
\alpha &= \sin^{-1}(0.864) = 59.77^{\circ} \\[1em]
\beta &= 180^{\circ} - (59.77^{\circ} + 70^{\circ}) = 50.23^{\circ}
\end{aligned}
$$

### 2.sor
$$
\begin{aligned}
a &= ? &&|&& \alpha = 110^{\circ} \\
b &= 12.4m &&|&& \beta = ? \\
c &= 8.3m &&|&& \gamma = ? \\[1em]
a^{2} &= b^{2} + c^{2} - 2bc \cdot \cos\alpha = 12.4^{\circ} + 8.3^{2} - 2 \cdot 12.4 \cdot 8.3 \cdot \cos110^{\circ} = 222.65 - 205.84 \cdot (-0.342) = 293 \\[.5em]
a &= \sqrt{293} = 17.12m \\[1em]
\sin\beta &= \frac{\sin\alpha}{a} \cdot b = \frac{\sin110^{\circ}}{17.12} \cdot 12.4 = 0.055 \cdot 12.4 = 0.682 \\[.5em]
\beta &= \sin^{-1}(0.682) = 43^{\circ} \\[1em]
\gamma &= 180^{\circ} - (43^{\circ} + 110^{\circ}) = 27^{\circ}
\end{aligned}
$$

### 3.sor
$$
\begin{aligned}
a &= 18dm &&|&& \alpha = ? \\
b &= ? &&|&& \beta = 69^{\circ} \\
c &= 120cm = 12dm &&|&& \gamma = ? \\[1em]
b^{2} &= a^{2} + c^{2} - 2ac \cdot \cos\beta = 18^{2} + 12^{2} - 2 \cdot 18 \cdot 12 \cdot \cos69^{\circ} = 468 - 432 \cdot 0.3583 = 468 - 154.79 = 313.21 \\[.5em]
b &= \sqrt{313.21} = 17.7dm \\[1em]
\sin\alpha &= \frac{\sin\beta}{b} \cdot a = \frac{\sin69^{\circ}}{17.7} \cdot 18 = \frac{0.9336}{17.7} \cdot 18 = 0.0527 \cdot 18 = 0.9468 \\[.5em]
\alpha &= \sin{-1}(0.9486) = 71.55^{\circ} \\[1em]
\gamma &= 180^{\circ} - (71.55^{\circ} + 69^{\circ}) = 39.45^{\circ}
\end{aligned}
$$

### Megoldás

$$
\begin{array}{|c|c|c|c|c|c|c|}
\hline
& a & b & c & \alpha & \beta & \gamma \\
\hline
\text{1. sor} & 9\text{ cm} & 8\text{ cm} & 9.79\text{ cm} & 59.77^\circ & 50.23^\circ & 70^\circ \\
\text{2. sor} & 17.12\text{ m} & 12.4\text{ m} & 8.3\text{ m} & 110^\circ & 43^\circ & 27^\circ \\
\text{3. sor} & 18\text{ dm} & 17.7\text{ dm} & 120\text{ cm} & 71.55^\circ & 69^\circ & 39.45^\circ \\
\hline
\end{array}
$$

---

[Vissza](../matematika.md)

---
