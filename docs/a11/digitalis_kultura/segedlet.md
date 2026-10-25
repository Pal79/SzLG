
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

---

[Vissza](../digitalis_kultura.md)

---

# Segédlet
## Az alap
A program alapfelépítése, ami sosem változik, csak bővítjük azt:
```cpp
#include <iosteram>

using namespace std;

int main() {

    return 0; // vagy return 1;
}
```
## Adatok kiíratása
Először csak egyszerű kiíratásokat hajtunk végre, később pedig már komplexebb adatokat tudunk majd közölni, eredményeket jelenítunnk meg.
```cpp
cout << "Helló, Világ!" << endl;
```
A kiíratás során a szövegben használhatunk olyan speciális vezérlő karaktereket, melyek valamilyen plusz funkciót adnak hozzá a kiíratáshoz. Ezeket a vezérlő karaktereket minden esetben `\` jellel (`backslash`) vezetjük be, ami a mögötte elhelyezkedő karakternek más jelentést ad.
- `\n` – sordobás (új sort kezd ennél a pontnál)
- `\t` – tabulátor (alapérték által meghatározott mezőnyit ugrik)
- `\b` – backspace (balra egy karakter visszatörlés)
- `\r` – visszaáll a kurzor a sor elejére, bármit írunk ezután, a sorban lévő szöveget törli
- `\a` – néhány terminálon esetleg megszólaltatja a gép speaker-jét
- `\\` – maga a `\` karakter
- `\"` – idézőjel

## Változók
Amikbe alapadatokat tárolunk, vagy a felhasználótól kérjük be az adatot, amivel esetleg feladatokat végzünk, vagy egyszerűen csak továbbadjuk a programnak:

- A változók neve egyedi kell hogy legyen (adott blokkon belül), csak betűvel kezdődhet, de utána bármennyi és bármilyen karakter állhat.
- A változók értéke alapvetően nem fix, ezt módosíthatjuk, erre utal a változó név. (léteznek fix változók is, melyek értékét csak egyszer adhatjuk meg.)
- Minden változó egy időpontban egyetlen értéket tárolhat. Ha új értéket adunk neki, az előző érték törlődik.

A változók használatával kapcsolatban két nagyon fontos fogalmat kell tisztázni:
- deklarálás: A deklarálás a változó típusának és nevének megadását jelenti. Ennek általános formája: `típus változónév;`
- inicializálás: Az inicializálás a változónak történő kezdőérték adás. Általános formája: `változónév = kezdőérték;`  
Ez a két lépés akár össze is vonható, ekkor a következőt írjuk: `típus változónév = kezdőérték;`

### Egész típusok (integer)
$$
\begin{array}{|l|l|l|l|}
\hline
\textbf{Típus} & \textbf{Leírás} & \textbf{Tárolás} & \textbf{Intervallum} \\
\hline
\text{short} & \text{rövid egész} & \text{16 bit} & \text{[-32768;32767]} \\
\text{int} & \text{egész} & \text{32 bit} & \text{[-2147483648;2147483647]} \\
\hline
\text{long} & \text{hosszú egész} & \text{32 bit} & \text{[-2147483648;2147483647]} \\
\text{long long} & \text{nagyon hosszú egész} & \text{64 bit} & \text{[-9223372036854775808;9223372036854775807]} \\
\hline
\end{array}
$$

> A tényleges méretek érdekében le tudod kérdezni őket: `sizeof(char), sizeof(short), sizeof(int), sizeof(long), sizeof(long long)`

### Lebegőpontos számok (float, double)
$$
\begin{array}{|l|l|l|}
\hline
\textbf{Típus} & \textbf{Leírás} & \textbf{Tárolás} \\
\hline
\text{float} & \text{egyszeres pontosságú lebegőpontos} & \text{32 bit} \\
\text{double} & \text{kétszeres pontosságú lebegőpontos} & \text{64 bit} \\
\hline
\end{array}
$$
#### Float
A lebegőpontos típusokat tört és valós számok ábrázolására használjuk:
- `float`: Mérete 4 bájt, pontossága 6-7 számjegy.
   - Használható: átlagszámítás, százalékok tárolása, gyors műveletek elvégzésére kevésbé pontos számokra
   - Hátránya: veszít a pontosságából
   - Mikor használjuk?
      - ha kevés memória is számít (pl. játékfejlesztésnél rengeteg koordinátát tárolsz)
      - ha nem kell nagyon nagy pontosság
      - ha gyors számítások kellenek

De a legtöbb hétköznapi programban inkább a double lesz a nyerő. 
#### Double
- `double`: Mérete 8 bájt, pontossága 15-16 számjegy

A legtöbb C++ programban a double az alapértelmezett választás, mert pontosabb, stabilabb, komolyabb számolásokhoz

A double is lebegőpontos, ezért néhány számot nem tud teljesen pontosan ábrázolni - de sokkal kevésbé pontatlan, mint a float.

### Bool típus - igaz, hamis
A bool (boolean) egy nagyon egyszerű, de mégis nagyon erős adattípus. Csak két értéke lehet:
- `true`: igaz - 1
- `false`: hamis - 0

Ahhoz, hogy ne `1`-et és `0`-t írjon ki, hanem a `true` vagy `false` szavakat, használjuk a `std::cout << std::boolalpha;` kifejezést.

## Operátorok és operandusok
A programozási nyelvek fontos részét képezik az operátorok. Programozás során sokszor úgynevezett kifejezésekkel dolgozunk, amelyek valamilyen értékek és közöttük értelmezett műveletek. Megnövelünk egy számot, összeadunk két változót, hogy egy harmadiknak megkapjuk az értékét, összehasonlítunk egy változót egy számmal, hogy egyenlőek-e, stb. Operátornak magát a műveletet nevezzük, operandusnak pedig a kifejezés azon részét, amit változtatni akarunk vagy amit felhasználunk a számításhoz. Az operandus lehet egy megadott literál (egy direkt érték), változó vagy kifejezés.
- `a = b;`
- `b == 2`
- `c = a + b;`
- `i++; (utónövekményes)`, `++i (előnövekményes)`
- `a += b * 2;`
- `c = a == 3 ? 0 : a;`

Az operátorokat következőképpen csoportosíthatjuk:
- egyoperandusú,
- kétoperandusú,
- többoperandusú operátor.  
Logikusabb azonban aszerint csoportosítani őket, hogy milyen jellegű műveletet hajtanak végre, bár vannak olyanok, amelyek nem sorolhatók be egyértelműen művelet alapján egy csoportba sem.
- Aritmetikai operátorok: `+`, `–`, `*`, `/`, `%`
- Relációs operátorok:
$$
\begin{array}{|l|l|}
\hline
\textbf{Reláció} & \textbf{Jele} \\
\hline
\text{kisebb} & \text{<} \\
\text{nagyobb} & \text{>} \\
\text{kisebb vagy egyenlő} & \text{<=} \\
\text{nagyobb vagy egyenlő} & \text{>=} \\
\text{egyenlő} & \text{==} \\
\text{nem egyenlő} & \text{!=} \\
\hline
\end{array}
$$
- Értékadó operátorok: `+=`, `-=`, `*=`, `/=`, `%=`
- Logikai operátorok:
   - negálás (tagadás): egy logikai kifejezés értékét az ellenkezőjére változtatja. Ami igaz volt, az hamis lesz, ami hamis volt, az igaz lesz. Vagy egy eldöntendő kérdést fordíthatunk meg vele.
      - Jelölése: `!`
      - Példák:
         - `!(szam % 2 == 0)` - nem páros
         - `!(szam > 5)` - nem nagyobb, mint 5
         - `!true` - nem igaz, tehát hamis
   - logikai és: A logikai és művelettel összekötött részfeltételek akkor adnak együtt igaz értéket, ha a kifejezés minden részfeltétele igaz.
      - Jelölése: `&&`
      - Példák:
         - `szam > 5 && szam % 2 == 0` - a szám 5-nél nagyobb ÉS páros
         - `szám < 0 && szam % 2 != 0` - a szám negatív ÉS páratlan
         - `szam > 10 && szam < 20` - a szám 10 ÉS 20 között van
   - logikai vagy: A logikai vagy művelettel összekötött részfeltételek akkor adnak együtt igaz értéket, ha a kifejezés legalább egy részfeltétele igaz.
   - Példák:
      - `szam > 0 || szam < 0` - a szám 0-nál nagyobb, VAGY 0-nál kisebb
      - `szam > 10 || szam < 0` - a szám 10-nél nagyobb vagy negatív
   - Kizáró vagy: A kizáró vagy akkor igaz, ha pontosan egy részfeltétele igaz. Ha a két dolog egyszerre nem fordulhat elő, akkor csak a kizáró vagy jöhet szóba.
      - Jelölése: `!=`
- Inkrementáló (növelő) operátorok
   - Létezik két speciális operátor, mely egy változó értékének 1-gyel való növelésére és csökkentésére szolgál:
      - utónövekményes: `i++` (postfix alak)
         - Példa: `int a = 10;`
            - `cout << a++ << endl;` -> 10
      - előnövekményes: `++i` (prefix alak)
         - Példa: `int a = 10;`
            - `cout << ++a << endl;` -> 11
- Feltételes operátor
   - Alakja: `feltétel ? ha_igaz : ha_hamis;`, a többit később
- Bitléptető és bitenkénti operátorok
   - Kicsit később


---

[Vissza](../digitalis_kultura.md)

---
