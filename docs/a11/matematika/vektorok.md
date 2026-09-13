
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
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

# Vektorok

Skaláris szorzat a koordináta rendszerben

![vektorok a koordináta rendszerben](../images/matematika-vektorok-001.svg)

Mivel a vektor párhuzamosan eltolható önmagával, ezért a kezdőpontja az origo.

## Paralelogramma szabály
A paralelogramma szabály két vektor összeadásának geometrikus módszere. Akkor a legcélszerűbb használni, ha a két vektor közös kezdőpontból indul.

### Az összegzés lépései
1. **Közös kezdőpont**: Helyezd el a két vektort ($a$ és $b$) úgy, hogy a kezdőpontjuk egybeessen ($O$ pont).
2. **Paralelogramma kiegészítés**: Rajzolj párhuzamos egyenest az $a$ vektor végpontján keresztül a $b$ vektorral, és a $b$ vektor végpontján keresztül az $a$ vektorral.
3. **Eredő vektor**: A közös kezdőpontból ($O$) a két párhuzamos egyenes metszéspontjába mutató átló adja a két vektor összegét ($c=a+b$).

![vektorok paralelogramma szyabály](../images/matematika-vektorok-paralelogramma-szabaly.svg)

A vektorok önmagukkal párhuzamosan eltolhatók.

![Vektorok párhuzamos eltolás](../images/matematika-vektorok-parhuzamos-eltolas.svg)

Megjegyzendő "szabály": vég mínusz kezdet

---

## Legfontosabb alapfogalmak és definíciók
- **Vektor**: Irányított szakasz. Rendelkezik nagysággal (hosszal), iránnyal és állással.
- **Vektor hossza (abszolút értéke / normája)**: A vektort ábrázoló szakasz hossza. Jelölése: $|a|$
- **Nullvektor**: Olyan vektor, amelynek a hossza $0$, és az iránya határozatlan (tetszőleges irányúnak tekinthető). Jelölése: $0$
- **Egységvektor**: Olyan vektor, amelynek a hossza pontosan 1 egység. Jelölése gyakran: $e$
- **Ellentett vektor**: Az $a$ vektor ellentettje az a $−a$ vektor, amelynek hossza és állása megegyezik $a$-éval, de az iránya ellentétes.
- **Egyenlő vektorok**: Két vektor egyenlő, ha a hosszuk és az irányuk is megegyezik (párhuzamos eltolással egymásba vihetők).
- **Egyállású (kollineáris) vektorok**: Olyan vektorok, amelyek párhuzamos egyeneseken vagy ugyanazon az egyenesen fekszenek.
- **Helyvektor**: A koordináta-rendszer origójából egy adott $P$ pontba mutató vektor. A helyvektor koordinátái megegyeznek a pont koordinátáival: $r_{p}=(x,y)$.
- **Skaláris szorzat**: Két vektor skaláris szorzata egy szám (skalár), amely a két vektor hosszának és a köztük lévő szög koszinuszának a szorzata: $a \cdot b = |a| \cdot |b| \cdot cos(\alpha)$.
- **Meredekségi / Irányvektor**: Egy egyenessel párhuzamos, nem nullvektor, amely kijelöli az egyenes irányát.
- **Normálvektor**: Egy adott egyenesre vagy síkra merőleges, nem nullvektor.

---
