
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

---

[Vissza](../matematika.md)

---
