
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

## Mi az a "Szemközti Pár"?
A szinusztétel a szemközti oldalak és szögek viszonyáról szól.
- `a` oldal és az $\alpha$ szög (egymással szemben vannak)
- `b` oldal és a $\beta$ szög (egymással szemben vannak)
- `c` oldal és a $\gamma$ szög (egymással szemben vannak)

**Aranyszabály**: A szinusztételt akkor és csak akkor tudod használni, ha a feladatban szereplő adatok között van legalább egy TELJES PÁR (azaz ismered az oldalt ÉS a vele szemközti szöget is)!

## Mikor mit csinálunk?
### Kiszámolni egy ismeretlen SZÖGET
Mikor használjuk?  
Ha ismersz egy teljes párt (pl. `a` és $\alpha$), plusz egy másik oldalt (pl. `b`), és annak a szemközti szögét ($\beta$) keresed.

Hogyan gondolkozzunk?
Írd fel a szinusztételt úgy, hogy az ismeretlen szög szinuszát egyedül hagyod az egyik oldalon:

$\sin\beta = \frac{b \cdot \sin\alpha}{a}$

Kiszámolod a jobb oldalt (kapsz egy $0$ és $1$ közötti tizedes törtet, pl. $0,522$).

A számológépen megnyomod a $\sin^{-1}$ (vagy arcsin) gombot, és megkapod a szöget fokban!

### Kiszámolni egy ismeretlen OLDALT
Mikor használjuk?  
Ha ismersz egy teljes párt (pl. `a` és $\alpha$), plusz egy másik szöget (pl. $\beta$), és annak a szemközti oldalát (`b`) keresed.

Hogyan gondolkozzunk?

Rámutatsz a keresett oldalra (`b`).

Átrendezed a képletet úgy, hogy a keresett oldal legyen balra:

$b = \frac{a \cdot \sin\beta}{\sin\alpha}$

**Tipp a megjegyzéshez**: A számlálóba (felülre) mindig a párja szinuszával megszorzott ismert oldal kerül, a nevezőbe (alulra) pedig a megmaradt szög szinuszai.

### A harmadik elem kiszámítása
Ha két szöged már megvan: Nincs szükség szinusztételre a harmadik szöghöz!

A háromszög szögeinek összege mindig $180^{\circ}$, így a harmadik szög egyszerüen:

$\gamma = 180 - (\alpha + \beta)$

Ha megvan a harmadik szög is: Akkor már kiszámolhatod a harmadik oldalt (c) is a B) ESET szerint!

## Feladatok előtt:
Tedd fel magának ezt a 3 kérdést sorban:
- Egyforma a mértékegység? (Pl. ha az egyik $dm$, a másik $cm$, először váltsuk át őket!)
- Megvan a teljes pár? (Pl. tudom az `a`-t és az $\alpha$-t is?)
	- Ha igen: Mehet a szinusztétel!
	- Ha nem: Akkor először a $180`{\circ}$-os szabályt kell használni, hogy meglegyen a hiányzó szög!

Mit keresek?
- Szöget? -> Szinusztétellel kiszámolom a szinuszát, aztán $sin^{-1}$.
- Oldalt? -> Szinusztétellel felírom a törtet, és összeszorzom/osztom.

---

[Vissza](../matematika.md)

---
