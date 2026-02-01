
---

[Vissza](../matematika.md)

---

# TRIGONOMETRIA
## Háromszög részei:
- `a` az **$\alpha$**-val szemközti befogó.
- `b` az **$\alpha$**-val szomszédos befogó
- `c` az átfogó

![derékszögű háromszög](../images/matematika-trigonometria.svg)
## Definíciók
### Szinusz
- A `szinusz` egy derékszögű háromszögben a szöggel szemközti befogó és az átfogó aránya. (hegycsúcsok magasságának a kiszámításához a mai napig használják).
    - $sin(\alpha)$ Megadja: szemközti befogó / átfogó $= \frac{a}{c}$ 
### Koszinusz
- A `koszinusz` a derékszögű háromszögben a szög melletti befogó és az átfogó aránya.
    - $cos(\alpha)$ megadja: szomszédos befogó / átfogó $= \frac{b}{c}$
### Tangens
- A `tangens` a befogókról szól: a szöggel szemközti és a szög melletti befogók arányát írja le.
    - $tan(\alpha)$ megadja: szemközti befogó / szomszédos befogó $=\frac{a}{b}$
### Kotangens
- A `kotangens` a tangens reciproka, vagyis a két befogó arányát fordítva adja meg.
    - $cot(\alpha)$ megadja: szomszédos befogó / szemközti befogó $=\frac{b}{a}$
## Mikor melyiket használjuk?
### Ha egy szög és az átfogó ismert $\implies$ szinusz vagy koszinusz
- `Szinusz`: ha a `szemközti befogó`t keresed:
    - $a = c \cdot sin(\alpha)$
- `Koszinusz`: ha a `szomszédos befogó`t keresed:
    - $b = c \cdot cos(\alpha)$
#### Tipikus feladatok:
- magasság számítása (pl. hegy, torony, antenna)
- létra dőlésszöge és hossza
- ferde sík feladatok
### Ha egy szög és egy befogó ismert $\implies$ tangens vagy kotangens
- `Tangens`: ha a `szemközti befogó`t akarod a szomszédosból
    - $a = b \cdot tan(\alpha)$
- `Kotangens`: ha a `szomszédos befogó`t akarod a szemköztiből
    - $b = a \cdot cot(\alpha)$
#### Tipikus feladatok:
- távolság–magasság összefüggések
- lejtők, rámpák, tetők dőlésszöge
- kamerák, reflektorok látószöge
### Ha két befogó ismert $\implies$ tangens vagy kotangens adja a szöget
- `Tangens`:
    - $\alpha = \arctan(\frac{a}{b})$
- `Kotangens`:
    - $\alpha = arccot \left (\frac{b}{a}\right)$
#### Tipikus feladatok:
- dőlésszög meghatározása
- emelkedők, lejtők meredeksége
- kamerák, antennák beállítása
### Ha egy befogó és az átfogó ismert $\implies$ szinusz vagy koszinusz adja a szöget
- `Szinusz`:
    - $\alpha = \arcsin(\frac{a}{c})$
- `Koszinusz`:
    - $\alpha = \arccos(\frac{b}{c})$
#### Tipikus feladatok:
- háromszög szögeinek meghatározása
- fizikai feladatok (erők felbontása)
- optikai szögek, beesési szögek
## Összefoglaló
- Szinusz $\implies$ szemközti / átfogó
- Koszinusz $\implies$ szomszédos / átfogó
- Tangens $\implies$ szemközti / szomszédos
- Kotangens $\implies$ szomszédos / szemközti

Ha átfogó van $\implies$ sin/cos  
Ha befogó van $\implies$ tan/cot  
Ha szöget keresel $\implies$ arcsin/arccos/arctan/arccot

## Feladatok / megoldás
1. feladat  
Egy derékszögű háromszög egyik befogója $a = 12\text{ cm}$, a hozzá tartozó szög pedig $\alpha = 35^\circ$.  
Számítsd ki a másik befogót.
- $a = 12 \text{cm}$
- $\alpha = 35^\circ$
- $b = ?$
    - $b = a \cdot cot(\alpha) = 12 \cdot cot(35) = 17.13777608\text{cm}$
2. feladat  
Egy létra $4\text{m}$ hosszú, és $70^\circ$-os szöget zár be a talajjal.  
Milyen magasra ér fel a falon?
- $c = 4\text{m}$
- $\alpha = 70^\circ$
- $a = ?$
    - $a = c \cdot sin(\alpha) = 4 \cdot sin(70) = 3.758770483\text{m}$
3. feladat  
Egy domb tetejéről egy autó $8^\circ$-os depressziószög alatt látszik. A domb magassága $30\text{m}$.  
Milyen messze van az autó a domb lábától?
- $\alpha = 8^\circ$
- $a = 30\text{m}$
- $b = ?$
    - $b = a \cdot cot(\alpha) = 30 \cdot cot(8) = 213.4610917\text{m}$
4. feladat  
Egy torony tetejéről egy templom tornya $12^\circ$-os emelkedési szög alatt látszik. A két torony közti vízszintes távolság $150\text{m}$.
Milyen magas a templom tornya, ha a megfigyelő torony $40\text{m}$ magas?

5. feladat  
Egy hajó $25^\circ$-os emelkedési szög alatt lát egy szikla tetejét. A hajó $180\text{m}$-re van a szikla lábától.  
Milyen magas a szikla?

6. feladat  
Egy háromszög két oldala:
$a = 18\text{ cm}$, $b = 25\text{ cm}$, és a közbezárt szög $\gamma = 47^\circ$.  
Számítsd ki a harmadik oldalt (koszinusztétel).

7. feladat  
Egy háromszögben:
$a = 12\text{ cm}$, $b = 15\text{ cm}$, $c = 17\text{ cm}$.  
Számítsd ki a legnagyobb szöget (koszinusztétel + trigonometria).

8. feladat  
Egy rádiótorony $60\text{m}$ magas. A torony tetejéről egy drótkötél a talaj egy pontjához csatlakozik úgy, hogy a kötél $40^\circ$-os szöget zár be a talajjal.  
Milyen hosszú a drótkötél?

9. Feladat  
Egy repülőgép $5^\circ$-os emelkedési szöggel emelkedik. Mekkora magasságot ér el $2\text{km}$ vízszintes megtétele után?

10. feladat  
Egy hegycsúcsot két különböző pontból figyelünk.  
Az első pontból a csúcs emelkedési szöge $18^\circ$, a második pontból (ami $300\text{m}$-el közelebb van a hegyhez) $25^\circ$.  
Milyen magas a hegy?

---

[Vissza](../matematika.md)

---