
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

---

# Trigonometria - összefoglaló
## Általános háromszög
A trigonometria a háromszögek szögeivel és oldalaival foglalkozik. 

### Szinusztétel
Bármely háromszögben két oldal aránya megegyezik a velük szemközti szögek szinuszainak arányával:
$$\frac{a}{b} = \frac{\sin\alpha}{\sin\beta}, \quad \frac{b}{c} = \frac{\sin\beta}{\sin\gamma}, \quad \frac{a}{c} = \frac{\sin\alpha}{\sin\gamma}$$

A tételekből az is következik, hogy az oldal és a vele szemközti szög szinuszának hányadosa a köré írható kör átmérőjét ($2R$) adja:
$$\frac{a}{\sin\alpha} = \frac{b}{\sin\beta} = \frac{c}{\sin\gamma} = 2R$$

### Koszinusztétel
Egy oldal négyzete megegyezik a másik két oldal négyzetének összegével csökkentve a két oldal és a közbezárt szög koszinuszának kétszeres szorzatát:
$$c^{2} = a^{2} + b^{2} - 2 \cdot a \cdot b \cdot \cos\gamma$$

## Derékszögű háromszög
Derékszögű háromszögben az egyik szög $90^{\circ}$, és az oldalak között az alábbi trigonometriai arányok érvényesek egy hegyesszög ($\alpha$) esetén:

- **Szinusz** (sin):
    - szöggel szemközti befogó / átfogó: $sin \alpha = \frac{a}{c}$
- **Koszinusz** (cos):
    - szög melletti befogó / átfogó: $cos \alpha = \frac{b}{c}$
- **Tangens** (tan):
    - szöggel szemközti befogó / szög melletti befogó: $tan \alpha = \frac{a}{b}$

### Fontos összefüggések derékszögű háromszögekre:
- $\sin^{2}\alpha + \cos^{2}\alpha = 1$
- $\tan\alpha = \frac{\sin\alpha}{\cos\alpha}$

---

## Háromszög területe és a beírható / köré írható körök sugara

### 1. Terület szinusz segítségével
Általános háromszög területét kiszámíthatjuk két oldal és a közbezárt szög segítségével:
$T = \frac{a \cdot b \cdot \sin\gamma}{2} = \frac{a \cdot c \cdot \sin\beta}{2} = \frac{b \cdot c \cdot \sin\alpha}{2}$

### 2. Köré írható kör sugara ($R$)
A háromszög területe kifejezhető a három oldal és a köré írható kör sugarának segítségével:
$T = \frac{a \cdot b \cdot c}{4R} \implies R = \frac{a \cdot b \cdot c}{4T}$

(A fent említett szinusztételből is kiszámítható: $R = \frac{a}{2\sin\alpha}$)

### 3. Beírható kör sugara ($r$)
A háromszög területe a félkerület ($s = \frac{a+b+c}{2}$) és a beírható kör sugarának szorzata:

$T = r \cdot s = r \cdot \frac{a+b+c}{2} \implies r = \frac{2T}{a+b+c}$

---
