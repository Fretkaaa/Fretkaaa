# 1. Jak zadeklarować zmienną w  C++ i jakie typy podstawowe są dostępne

Deklaracja zmiennej polega na podaniu typu i nazwy zmiennej
typy  podstawowe: int, bool, double, float, string, char

# 2. Jak zainicjować zmienną

Wystarczy dodać wartość do zmiennej
```cpp
int a = 10;
```
# 3. Jaka jest różnica między zmienną lokalną a globalną

Zmienna lokalna jest dostępna tylko w danej klasie, globalna jest dostępna w całym kodzie (można sie do niej odniesc wszedzie)

# 4. Co oznacza słowo kluczowe const przy deklaracji zmiennej

```Const``` to stała, nie zmienia wartości

# 5. Czym jest instrukcja warunkowa

pozwala na wykonanie różnych bloków kodu w zależności od tego, czy wyrażenie logiczne jest prawdziwe czy fałszywe

# 6. Czym jest klasa w C++ i do czego służy

Klasa jest mechanizmem tworzenia typów danych zdefiniowanych przez użytkownika

# 7. Czym różni się klasa od obiektu

Klasa to szablon, który definiuje cechy (dane, atrybuty) i zachowania (metody, funkcje) obiektów danego typu. Obiekt to konkretna, rzeczywista instancja (np. konkretny samochód) tej klasy

# 8. Jak zdefiniować klasę w  C++ i jak utworzyć jej obiekt
```cpp
#include <iostream>
using namespace std;

class Samochod {
public:
    string marka;
    int rok;

    void przedstawSie() {
        cout << "Samochod: " << marka << ", rok: " << rok << endl;
    }
};

int main() {
    Samochod auto1;   // obiekt klasy Samochod; auto2 to nazwa obiektu klasy Samochod
    auto1.marka = "Toyota";
    auto1.rok = 2020;

    Samochod auto2;   // drugi obiekt
    auto2.marka = "BMW";
    auto2.rok = 2018;

    auto1.przedstawSie();
    auto2.przedstawSie();

    return 0;
}
```
# 9. Co to są specyfikatory dostępu (public, private, protected) i jakie mają znaczenie

```public``` zapewnia dostęp zewsząd
```private``` ogranicza dostęp tylko do wnętrza samej klasy
```protected``` pozwala na dostęp zarówno z wnętrza klasy, jak i z jej klas pochodnych.

# 10.  Do czego służą konstruktory i destruktory w klasie

Konstruktor to metoda uruchamiania przy tworzeniu obiektu do jego inicjalizacji, a destruktor to metoda wywoływana przy niszczeniu obietku do zwalniania zasobów

# 11. Co oznacza słowo kluczowe this w klasie

```this``` to wskaźnik na aktualny obiekt używany np. w odróżnieniu pól klasy od parametrów funkcji lub zwracania samego obiektu w metodach

# 12. Czym jest tablica i jak ją zadeklarować

zmienna przechowująca wiele elementów, danych.

```cpp
int liczby[5] = {10, 20, 30, 40, 50};
```
