
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

Az előző órán tanultuk, hogy hogyan kell felépteni egy `c++` program alapjait:
```cpp
#include <iostream>

using namespace std;

int main() {

  return 0; // vagy return 1;
}
```

Ha az elején nem írtuk be a `using namespace std;`-t, akkor a `std::` előtagot is használnunk kell: `std::cout << "Kiírandó szöveg vagy szám" << std::endl;`.

A programnak adatot pedig így adhatunk meg bemenetnek: `cin >> bemenet;`.

---

A mai órán viszont már nem csak egyszerűen kiírunk valamit, hanem meg is vizsgálunk egy változó értékét, majd kiírjuk az eredményt:

`primtényezős felbontás`:
```cpp
#include <iostream>

using namespace std;

int main() {

    int num;

    cout <<"Írj be egy egész számot: ";
    cin >> num;

    cout <<"\n\nA(z) " << num <<" osztói a négyzetgyökig:" << endl;
    for(int i = 2; i<=num/i; i++) {
        if(num % i == 0) {
            cout << i <<" és " << (num/i) << endl;
        }
    }

    return 0;

}
```
Ez így gondolom nem mond még sokat nektek, ezért megpróbálom leírni, hogy mi is történik.
1. ez a kód egy beírt szám összes osztóját kiírja, viszont nem fut végig egészen a számig, hanem megáll a négyzetgyökénél.
1. szám bekérés:
   - létrehozunk egy `num` nevű változót
   - majd kérünk egy számot a konzolról
1. Miért `i <= num/i` a ciklusban?
   - Ha meg akarjuk keresni a 36 osztóit, nem kell elszámolni 1-36-ig. Ha találunk egy osztót, mondjuk a 4-et (36/4=9), akkor a 9 is automatikusan osztó.
   - A `i <= num/i` pont ugyanazt jelenti, mint `i * i <= num`, viszont így a program gyorsabban fut le, mert csak a négyzetgyökig fut.
1. Osztók vizsgálata és kiírás (`if` ág)
   - a `num % i == 0` azt vizsgálja, hogy az `i` maradék nélkül osztja e a számot, tehát osztó e.
   - ha igen, akkor rögtön két osztót is tudunk kiírni egyszerre: magát az `i`-t és a `num/i`-t
   - Ha `num = 36` és `i = 4`, akkor a program kiírja, hogy `4 és 9`.

---

[Vissza](../digitalis_kultura.md)

---
