
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

# Féléves vizsga
## Számtani és mértani közép
### Számtani közép (két szám átlaga)
Képlete: $a_{k} = \frac{a+b}{2}$

### Mértani közép (két nemnegatív szám szorzatának négyzetgyöke)
Képlete: $g = \sqrt{a \cdot b}$
#### Tétel
Két szám számtani közepe mindig nagyobb vagy egyenlő, mint a mértani közepük ($a_{k} \ge g$).

#### Példa:
$$
\begin{aligned}
a &= 4 \\
b &= 9 \\[2em]
a_{k} &= \frac{4+9}{2}=6.5 \\
g &= \sqrt{4\cdot9}=6
\end{aligned}
$$

## 2210 feladat
### a.
$$
\begin{aligned}
a &= 3 \\
b &= 27 \\[2em]
a_{k} &= \frac{3+27}{2}=15 \\
g &= \sqrt{3 \cdot 27}=9
\end{aligned}
$$

### b.
$$
\begin{aligned}
a &= 12 \\
b &= 27 \\[2em]
a_{k} &= \frac{12+27}{2}=19.5 \\
g &= \sqrt{12 \cdot 27}=18
\end{aligned}
$$

### c.
$$
\begin{aligned}
a &= 20 \\
b &= 45 \\[2em]
a_{k} &= \frac{20+45}{2}=32.5 \\
g &= \sqrt{20 \cdot 45}=30
\end{aligned}
$$

### d.
$$
\begin{aligned}
a &= 40 \\
b &= 90 \\[2em]
a_{k} &= \frac{40+90}{2}=65 \\
g &= \sqrt{40 \cdot 90}=60
\end{aligned}
$$

---

## Másodfokú egyenlet megoldóképlete
Az $ax^{2}+bx+c=0$ alakú egyenletek megoldására szolgál.
### Képlet
$x_{1,2} = \frac{ -b \pm \sqrt{b^{2} -4 \cdot a\cdot c}}{2 \cdot a}$
#### Példa:
$$
\begin{aligned}
& x^{2}-5x+6 = 0 \\[2em]
a &= 1 \\
b &= -5 \\
c &= 6 \\[2em]
& \text{Behelyettesítés:} \\[1em]
x_{1,2} &= \frac{5\pm \sqrt{25-24}}{2} = \\
x_{1} &= 3 \\
x_{2} &= 2
\end{aligned}
$$

## Gyöktényezős vagy szorzat alak
Ha az egyenlet gyökei $x_{1}$ és $x_{2}$, akkor a másodfokú kifejezés felírható szorzatként.
### Alak:
$a(x-x_{1})(x-x_{2})=0$
### Példa:
Ha a gyökök $2$ és $3$, az egyenlet: $(x-2)(x-3)=0$
### 2168. feladat
#### a.
$$
\begin{aligned}
& x^{2}+x-6 \\
& x^{2}+5x+6 \\[2em]
a &= 1 \\
b &= 5 \\
c &= 6 \\[2em]
x_{1,2} &= \frac{-5 \pm \sqrt{5^{2} - 4 \cdot 1 \cdot 6}}{2 \cdot 1} = \\
& D = 5^{2} - 4 \cdot 1 \cdot 6 = 1 \\
&= \frac{-5 \pm  \sqrt{1}}{2} = \\
x_{1} &= \frac{-5+1}{2} = \frac{-4}{2} = -2 \\
x_{2} &= \frac{-5-1}{2} = \frac{-6}{2} = -3 \\
&\text{Szorzattá alakítás:} \\
&(x+2)(x+3)
\end{aligned}
$$

#### b.
$$
\begin{aligned}
& x^{2}−2x−8 \\[2em]
a &= 1 \\
b &= -2 \\
c &= -8 \\[2em]
x_{1,2} &= \frac{2 \pm \sqrt{(-2)^{2} - 4 \cdot 1 \cdot (-8)}}{2 \cdot 1} = \\
& D = (-2)^{2} - 4 \cdot 1 \cdot (-8) = 36 \\
& \frac{2 \pm \sqrt{36}}{2} \\
x_{1} &= \frac{2 + \sqrt{36}}{2} = \frac{8}{2} = 4 \\
x_{2} &= \frac{2 - \sqrt{36}}{2} =  \frac{-4}{2} = -2 \\
& \text{Szorzattá alakítás:} \\
& (x-4)(x+2)
\end{aligned}
$$

#### c.
$$
\begin{aligned}
& x^{2}−6x+5 \\[2em]
a &= 1 \\
b &= (-6) \\
c &= 5 \\[2em]
x_{1,2} &= \frac{6 \pm \sqrt{(-6)^{2} - 4 \cdot 1 \cdot 5 }}{2 \cdot 1} = \\
& D = (-6)^{2} - 4 \cdot 1 \cdot 5 = 16 \\
& \frac{6 \pm \sqrt{16}}{2} = \\
x_{1} &= \frac{6 + \sqrt{16}}{2} = \frac{10}{2} = 5 \\
x_{2} &= \frac{6 - \sqrt{16}}{2} = \frac{2}{2} = 1 \\
& \text{Szorzattá alakítás:} \\
& (x - 5)(x - 1)
\end{aligned}
$$

### 2169 feladat
#### a.
$$
\begin{aligned}
& 3 \text{ és } 4 \\[2em]
& (x-3)(x-4)=x^{2}-4x-3x+12=x^{2}-7x+12
\end{aligned}
$$

#### b.
$$
\begin{aligned}
& -2 \text{ és } 7 \\[2em]
& (x+2)(x-7)=x^{2}-7x+2x-14=x^{2}-5x-14
\end{aligned}
$$

#### c.
$$
\begin{aligned}
& -3 \text{ és } -6 \\[2em]
& (x+3)(x+6)=x^{2}+6x+3x+18=x^{2}+9x+18
\end{aligned}
$$

#### d.
$$
\begin{aligned}
& 1 \text{ és } -5 \\[2em]
& (x-1)(x+5)=x^{2}+5x-x-5=x^{2}+4x-5
\end{aligned}
$$

## Teljes négyzetalak
A kifejezést $(x \pm d)^{2}+e$ alakra hozzuk. Ez segít a függvény ábrázolásánál (szélsőérték keresésnél).
### Példa:
$x^{2}+6x+10=(x+3)^{2}-9+10=(x+3)^{2}+1$

## Másodfokú visszavezethető magasabb fokszámú egyenletek
Olyan egyenletek (pl. negyedfokú), ahol új változót vezetünk be (helyettesítés).
### Példa:
$$
\begin{aligned}
& x^{4}−5x^{2}+4 = 0 \\[2em]
& \text{Legyen } a = x^{2} \\[2em]
& \text{Ekkor } a^{2} − 5a + 4 = 0 \\[2em]
& \text{Megoldjuk } a\text{-ra } ($a1​=1,a2​=4$) \\[2em]
& \text{majd visszatérünk }x\text{-re: } x^{2}=1 \Rightarrow x=\pm 1$ és $x2=4 \Rightarrow x=\pm 2
\end{aligned}
$$

## Másodfokú egyenlőtlenségek
Itt nem csak pontokat (gyököket) keresünk, hanem tartományokat.

Lépések:
1. Nullára rendezzük.
1. Megoldjuk egyenletként.
1. Vázoljuk a parabolát és leolvassuk a tartományt (hol van a tengely felett/alatt).

### Példa:
$$
\begin{aligned}
& x^{2} − 4 < 0 \\[2em]
& \text{A gyökök }−2\text{ és }2 \\[2em]
& \text{Mivel a parabola felfelé nyitott, a megoldás: }−2 < x < 2
\end{aligned}
$$

## Négyzetgyökös egyenletek
Ahol az ismeretlen a gyökjel alatt van.
- Fontos: Mindig kell értelmezési tartomány (gyök alatt nem állhat negatív) és a végén ellenőrzés (a négyzetre emelés miatt hamis gyökök keletkezhetnek).
### Példa:
$x+2​=3 \implies x+2=9 \implies x=7$.

## Diszkrimináns fogalma
A megoldóképletben a gyök alatti kifejezés:

$D = b^{2}-4\cdot a\cdot c$

ez határozza meg a megoldások számát.
- Ha $D>0$: két különböző megoldás

![diszkrimináns 1](../images/matematika-diszkriminans-001.svg)

- Ha $D=0$: egy valós megoldás (két egybeeső)

![diszkirmináns 2](../images/matematika-diszkriminans-002.svg)

- Ha $D < 0$: nincs valós megoldás

![diszkrimináns 3](../images/matematika-diszkriminans-003.svg)

## Másodfokú függvény
Az $f(x)=ax^{2}+bx+c$ függvény grafikonja egy parabola.
- Ha $a > 0$, a parabola felfelé nyitott (minimuma van).
- Ha $a < 0$, lefelé nyitott (maximuma van).

## Szöveges egyenletek
Olyan feladatok, ahol a szöveg alapján kell felállítani egy másodfokú egyenletet. Gyakori témák: számok kapcsolata, téglalap oldalai, munkavégzés.
- **Tipp**: Jelöld el az egyik ismeretlent x-szel, és a többit írd fel ennek segítségével.

---

[Vissza](../matematika.md)

---
