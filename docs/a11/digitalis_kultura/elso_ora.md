
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

# Bevezetés a C++ programozásba
## Mi az a C++?
A `C++` a világ egyik legnépszerűbb, leghatékonyabb és legelterjedtebb programozási nyelve. **Bjarne Stroustrup** hozta létre 1979-ben a korábbi, `C` nevű nyelv továbbfejlesztéseként (innen ered a neve is: a `++` a programozásban a növelést, lépést jelenti).
### Miért pont a C++ nyelvet tanuljuk?
- **Rendkívül gyors**: A `C++` kód közvetlenül a számítógép hardverével kommunikál, így szinte az egyik leggyorsabb nyelv a világon.
- **Ezzel készülnek játékok**: A legtöbb nagy, modern videojáték-motor (például az `Unreal Engine`) és a `AAA`-kategóriás játékok (pl. `GTA V`, `Counter-Strike`, `Minecraft C++ verziója`) `C++` nyelven íródnak.
- **A való élet rendszerei ezen futnak**: Az önvezető autók, az űrhajók szoftverei, az operációs rendszerek (`Windows`, `macOS`) és a böngészők (`Chrome`) alapja is a `C++`.
- **Fejleszti a logikát**: Ha megtanulod a `C++` működését, utána bármilyen más programozási nyelvet (`Python`, `JavaScript`, `Java`) pillanatok alatt meg fogsz érteni!
### Hogyan működik a C++ program?
1. **Megírjuk a kódot**: Ez egy szöveges fájl (a mi utasításaink a számítógépnek).
1. **Lefordítjuk (Fordítás / Compilation)**: A számítógép nem érti az emberi szöveget, csak a gépi kódot (nullákat és egyeseket: $01001000...$). Egy fordítóprogram (`compiler`) átalakítja a megírt kódunkat gépi nyelvre.
1. **Futtatjuk**: A számítógép végrehajtja a lefordított utasításokat.

## Alap program felépítése
- `#include <iostream>`: Be - és kimeneti műveletekhez (pl. `cout`) szükséges könyvtár
- `#include <windows.h>`: Az ékezetes karakterek helyes megjelentéséhez (Windows alatt)
- `using namespace std;`: Hogy ne kelljen kiírni az `std::` előtagot (pl. `std::cout` helyett elég a `cout`)
- `int main()`: A főfüggvény: itt kezdődik a program végrehajtása
    - `SetConsoleOutputCP(1250);`: Kimeneti kódlap beállítása (Windows)
    - `SetConsoleCP(1250);`:  Bemeneti kódlap beállítása (Windows)
    - `cout << "Árvíztűrő Tükörfúrógép" << endl;`: Szöveg kiíratása és soremelés (`endl`)
    - `return 0;`: A 0 jelezze a rendszernek, hogy a program hiba nélkül lefutott

- **Dupla perjelek (`//`)**: Kommentek, amiket a fordító figyelmen kívül hagy, csak a programozónak szólnak.
- **Pontosvessző (`;`)**: A C++ utasítások végét jelzi (mint a mondat végén a pont).
- **Kapcsos zárójelek (`{ }`)**: A kódblokkot jelölik, ami a `main()` függvényhez is tartozik

### Egyszerű kiíratás:
```cpp
#include <iostream>
#include <windows.h> // csak windows-nál

using namespace std;

int main() {
    SetConsoleOutputCP(1250);
    SetConsoleCP(1250);

    cout << "Árvíztűrő Tükörfúrógép" << endl;

    return 0;
}
```

### Egyszerű matematikai program (csak összeadás):
```cpp
#include <iostream>
#include <windows.h> // csak windows-nál

using namespace std;

int main() {
    SetConsoleOutputCP(1250);
    SetConsoleCP(1250);

    // 1. VÁLTOZÓK LÉTREHOZÁSA (deklaráció)
    // Az 'int' azt jelenti, hogy egész számokat fogunk tárolni bennük
    int x;
    int y;

    // 2. ELSŐ SZÁM BEKÉRÉSE
    cout << "Írd be az x értékét: " << endl; // Üzenet a felhasználónak
    cin >> x; // A beírt érték elmentése az x változóba (változó definiálása)

    // 3. MÁSODIK SZÁM BEKÉRÉSE
    cout << "Írd be az y értékét: " << endl;
    cin >> y; // A beírt érték elmentése az y változóba

    // 4. EREDMÉNY KIÍRATÁSA
    // Összeadjuk a két változót, és azonnal kiírjuk az eredményt
    cout << "A két szám összege: " << x + y << endl;
    
    return 0; // Jelzés a rendszernek: a program hiba nélkül lefutott
}
```

---

[Vissza](../digitalis_kultura.md)

---
