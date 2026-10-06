
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

## Szinusztétel
Tetszőleges háromszögben:
$$
\begin{aligned}
\frac{a}{\sin \alpha} &= \frac{b}{\sin \beta} = \frac{c}{\sin \gamma}
\end{aligned}
$$

Mit mond ki?  
Egy oldal hossza arányos a szemközti szög szinuszával.

Mikor használjuk?
- Ha két szög + egy oldal adott
- Ha két oldal + egy nem közbezárt szög adott
- Ha hiányzik egy szög vagy egy oldal, és könnyen pótolható

## Koszinusztétel
Tetszőleges háromszögben:
$$
\begin{aligned}
c^{2} &= a^{2} + b^{2} - 2ab \cdot \cos(\gamma)
\end{aligned}
$$

Hasonlóképpen:
$$
\begin{aligned}
a^{2} &= b^{2} + c^{2} - 2bc \cdot \cos(\alpha) \\[1em]
b^{2} = a^{2} + c^{2} - 2ac \cdot \cos(\beta)
\end{aligned}
$$

Mit mond ki?  
A harmadik oldal négyzete = két oldal négyzetének összege – kétszer a szorzatuk és a közbezárt szög koszinuszának szorzata.

Mikor használjuk?
- Ha két oldal + közbezárt szög adott
- Ha három oldal adott $\implies$ szöget keresünk

## Tangens tétel
Tetszőleges háromszögben:
$$
\begin{aligned}
\frac{a - b}{a + b} &= \frac{\tan\left(\frac{\alpha - \beta}{2}\right)}{\tan\left(\frac{\alpha + \beta}{2}\right)}
\end{aligned}
$$

Mit mond ki?  
Két oldal különbségének és összegének aránya kapcsolatban van a szemközti szögek félösszegének és félkülönbségének tangensével.

Mikor használjuk?
- Ritkábban kell, de hasznos, ha két oldal és két szög közötti kapcsolatot keresünk
- Olyan feladatoknál, ahol fél-szögek jelennek meg

## Kotangens tétel
Tetszőleges háromszögben:
$$
\begin{aligned}
\cot\gamma &= \frac{a^2 + b^2 - c^2}{4T}
\end{aligned}
$$

ahol T a háromszög területe.

Másik alakja:
$$
\begin{aligned}
\cot(\gamma) &= \frac{a \cdot \cos(\beta) + b \cdot \cos(\alpha)}{a \cdot \sin(\beta) + b \cdot \sin(\alpha)}
\end{aligned}
$$

Mit mond ki?  
A kotangens a háromszög oldalai és területe között teremt kapcsolatot.

Mikor használjuk?
- Haladóbb feladatoknál
- Terület–szög–oldal összefüggéseknél
- Trigonometrikus átalakításoknál

## Összefoglaló
$$
\begin{array}{|l|l|l|}
\hline
\text{Szinusz tétel} & \frac{a}{\sin \alpha} = \frac{b}{\sin \beta} = \frac{c}{\sin \gamma} & \text{Oldal-szög arányok} \\
\hline
\text{Koszinusz tétel} & c^{2} = a^{2} + b^{2} - 2ab \cdot \cos(\gamma) & \text{Oldal vagy szög számítása} \\
\hline
\text{Tangens tétel} & \frac{a - b}{a + b} = \frac{\tan\left(\frac{\alpha - \beta}{2}\right)}{\tan\left(\frac{\alpha + \beta}{2}\right)} & \text{Fél-szöges összefüggések} \\
\hline
\text{Kotangens tétel} & \cot\gamma = \frac{a^{2} + b^{2} - c^{2}}{4T} & Terület-szög-oldal kapcsolat \\
\hline
\end{array}
$$

---

[Vissza](./trigonometria.md)

---
