
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
## Változók használata
Amikbe alapadatokat tárolunk, vagy a felhasználótól kérjük be az adatot, amivel esetleg feladatokat végzünk, vagy egyszerűen csak továbbadjuk a programnak:

### Egész típusok (integer)
$$
\begin{array}{|l|l|l|l|}
\hline
\textbf{Típus} & \textbf{Jellemző méret (8 bites bájttal)} & \textbf{Előjeles (signed) tartomány} & \textbf{Előjel nélküli (unsigned) tartomány} \\
\hline
\text{char} & \text{1 bájt} & \text{-128...127} & \text{0...255} \\
\hline
\text{short} & \text{2 bájt} & \text{-32768...32767} & \text{0...65535} \\
\hline
\text{int} & \text{4 bájt} & \text{-2 147 483 648 … 2 147 483 647} & \text{0 … 4 294 967 295} \\
\hline
\text{long} & \text{legalább 4 bájt} & \text{rendszerfüggő} & \text{rendszerfüggő} \\
\hline
\text{long long} & \text{legalább 8 bájt} & \text{nagyon nagy tartomány} & \text{még nagyobb} \\
\hline
\end{array}
$$
> A tényleges méretek érdekében le tudod kérdezni őket: `sizeof(char), sizeof(short), sizeof(int), sizeof(long), sizeof(long long)`

### Lebegőpontos számok (float, double)
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

---

[Vissza](../digitalis_kultura.md)

---
