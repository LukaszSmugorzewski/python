Ćw 10

# =====================================================================LISTY================================================================================
lista = [1,2,3,4,"wow","XD",True,"nigger","reggin",9]
lista[1] = 5
print(lista)
print(tuple(lista)[7])
print(lista[::-2])
print(lista[-4])

def funckja(a,b,c,d,e,f,g):
    lista = [a,b,c,d,e,f,g]
    if a > b and b > c and c > d and d > e and e > f and f > g:
        return True
    else:
        return False

print(funckja(6,5,4,4,2,1,0))

def funkcja(a,b,c,d,):
    lista1 = [a,b]
    lista2 = [c,d]
    print(lista1), print(lista2)
    wynik = [a + c,d + b]
    return wynik

print(funkcja(1,2,3,4))

def func(lista, n1, n2):
    for i in range(len(lista)):
        if lista[i] == n1:
            lista[i] = n2
    return lista

numer = int(input("wpisz jak dluga ma być twoja lista:"))
lista = []
for _ in range(numer):
    element = int(input("wpisz swoją listę: "))
    lista.append((element))
n1 = int(input("wpisz jaka liczbe chcesz zamienić: "))
n2 = int(input("na jaką liczbę chcesz zamienić: "))
print("orginalna lista", lista)
print("zmieniona lista", func(lista, n1, n2))

def func(lista, n1, n2):
    for i in range(len(lista)):
        if lista[i] == n1:
            lista[i] = n2


numer = int(input("wpisz jak dluga ma być twoja lista:"))
lista = []
for _ in range(numer):
    element = int(input("wpisz swoją listę: "))
    lista.append(element)
n1 = int(input("wpisz jaka liczbe chcesz zamienić: "))
n2 = int(input("na jaką liczbę chcesz zamienić: "))
print("orginalna lista", lista)
func(lista, n1, n2)
print("zmieniona lista", lista)

def func(lista, n1, n2):
    for i in range(len(lista)):
        if lista[i] isclose:
            lista[i] = n2
    return lista

numer = int(input("wpisz jak dluga ma być twoja lista:"))
lista = []
for _ in range(numer):
    element = int(input("wpisz swoją listę: "))
    lista.append((element))
n1 = int(input("wpisz jaka liczbe chcesz zamienić: "))
n2 = int(input("na jaką liczbę chcesz zamienić: "))
print("orginalna lista", lista)
print("zmieniona lista", func(lista, n1, n2))

from math import isclose

def func(lista, n1, n2):
    for i in range(len(lista)):
        if isclose(lista[i], n1, rel_tol=0.5):
            lista[i] = n2
    return lista

numer = int(input("wpisz jak dluga ma być twoja lista: "))
lista = []
for _ in range(numer):
    element = float(input("wpisz swoją listę: "))
    lista.append((element))
n1 = float(input("wpisz jaka liczbe chcesz zamienić: "))
n2 = float(input("na jaką liczbę chcesz zamienić: "))
print("orginalna lista", lista)
print("zmieniona lista", func(lista, n1, n2))

==========================================================================KROTKI===========================================================

krotka = (1,2,3,4,'abc','def',True)

print(krotka[3])
print(krotka[3:6])
print(krotka[-3])

def funkcja(krotka,element):
    nowa_krotka1= krotka+ (element,)

    lista = list(krotka)
    lista.append(element)
    nowa_krotka2 = tuple(lista)

    return nowa_krotka2, nowa_krotka1

krotka = (1,2,3)
element = 4

nowa_krotka1, nowa_krotka2 = funkcja(krotka,element)

print("pierwsza krotka: ", nowa_krotka1)
print("druga krotka: ", nowa_krotka2)

def bez_powtórzeń(lista):
    nowa_krotka = set(lista)
    print("twoja nowa krotka", nowa_krotka)

bez_powtórzeń((1,2,3,4,2,1,2,3,4,5,6,4,7,))

===========================================================LIST COMPREHENSIONS=====================================================


potęgi = [5 ** x for x in range(14)]
print(potęgi)


n = 3
silnia = eval("*".join([str(i) for i in range(1, n + 1)]))
print(silnia)


lista = [x" for x in range(9)
lista[0] = 1
print(lista)

nowalista = []
lista = ['kowalski', 'nowak', 'makasza', 'wow', 'makumba', 'el']
for i in range(len(lista)):
    if len(lista[i]) > 5:
        nowalista.append(lista[i])
print(nowalista)



def funkcja(lista):
    wynik = [x ** 3 for x in lista if x % 2 == 0]
    return wynik

lista = [1,2,3,4,5,6,7,8]
print(funkcja(lista))

a = ""
names = ["michal", "nela", "ola", "przemek"]
for i in range(len(names)):
    a += names[i]

print(len(a))

names = ["michal", "nela", "ola", "przemek", 'lana']
names = [name.capitalize() for name in names]
print(names)

names = ["michal", "nela", "ola", "przemek"]
names_with_l = [name for name in names if 'l' in name.lower()]
print(names_with_l)

names = ["michal", "nela", "ola", "przemek"]
kobiety = [name.capitalize() for name in names if name.endswith('a')]
print(kobiety)

==============================================================================ĆW 11=============================================================

============================================================================SET=================================================================
slownik = {"Polska","Niemcy","Belgia","Anglia","Ukraina"}
if "Polska" in slownik:
    print("polska jest w slowniku")

slownik.remove("Polska")
print(slownik)

slownik.add(("francja"))
print(slownik)

===================================================================słowniki====================================================================

zbiór1 = {'szczytno','marbork','radom'}
zbiór2 = {'szczytno','szczecin','warszawa'}

print(zbiór1 | zbiór2)
print(zbiór1 & zbiór2)
print(zbiór1 - zbiór2)
print(zbiór1 ^ zbiór2)

słownik = {}
a = int(input("wpisz ile chcesz dodać rekordów: "))
for i in range(a):
    b = input("wpisz klucz: ")
    c = input("wpisz wartość: ")
    słownik.update({b : c})
def print_phone_numbers(słownik):
    for i in słownik:
        print(f"{i} ma numer {słownik.get(i)}")
print_phone_numbers(słownik)

slownik = {1: "Poniedziałek", 2: "Wtorek", 8: "Niedziela"}

print(slownik[1])
print(slownik[2])
slownik[3] = "Środa"
slownik[4] = False
slownik[5] = 5
print(slownik)
slownik["a"] = 1
print(slownik['a'])
print(slownik)

print(slownik[])
print(slownik.get(8, "inny dzień"))

print("\nPętka:")

for i in slownik.values():
    print(i)

print("---------")
print(slownik.pop(3))
print(slownik)

zbiór1 = {'szczytno','marbork','radom'}
zbiór2 = {'szczytno','szczecin','warszawa'}

print(zbiór1 | zbiór2)
print(zbiór1 & zbiór2)
print(zbiór1 - zbiór2)
print(zbiór1 ^ zbiór2)

słownik = {}
a = int(input("wpisz ile chcesz dodać rekordów: "))
for i in range(a):
    b = input("wpisz klucz: ")
    c = input("wpisz wartość: ")
    słownik.update({b : c})
def print_phone_numbers(słownik):
    for i in słownik:
        print(f"{i} ma numer {słownik.get(i)}")
print_phone_numbers(słownik)

def translate_en_to_pl(dni_tygodnia_en):
    dni_tygodnia_pl = {"Monday":"Poniedziałek","Tuesday":"Wtorek","Wednesday":"środa","Thursday":"czwartek","Friday":"Piątek","Saturday":"Sobota","sunday":"Niedziela"}
    return [dni_tygodnia_pl[day] for day in dni_tygodnia_en if day in dni_tygodnia_pl]

dni_tygodnia_en = ["Monday","Thursday","Wednesday"]
dni_tygodnia_pl = translate_en_to_pl(dni_tygodnia_en)
print(dni_tygodnia_pl)

def translate_pl_to_en(dni_tygodnia_en):
    dni_tygodnia_en = {"Poniedziałek":"Monday","Wtorek":"Tuesday","Środa":"Wednesday","Czwartek":"Thursday","Piątek":"Friday","Sobota":"Saturday","Niedziela":"Sunday"}
    return [dni_tygodnia_en[day] for day in dni_tygodnia_pl if day in dni_tygodnia_en]

dni_tygodnia_pl = ["Środa","Sobota"]
dni_tygodnia_en = translate_pl_to_en(dni_tygodnia_pl)
print(dni_tygodnia_en)

def segregator(lista):
    miesiące = {1: "Styczeń", 2: "Luty", 3: "Marzec", 4: "Kwiecień", 5: "Maj", 6: "Czerwiec", 7: "Lipiec",
                8: "Sierpień", 9: "Wrzesień", 10: "Październik", 11: "Listopad", 12: "Grudzień"}
    nowa_lista = []
    for i in lista:
        if i in miesiące.values():
            nowa_lista.append(i)
    nowa_lista.sort(key=lambda x: list(miesiące.values()).index(x)) # sortowanie według indexu
    return nowa_lista

lista = []
a = int(input("Wpisz ile słów ma miec twoja lista: "))
for i in range(a):
    b = input("Wpisz nazwe miesiąca: ")
    lista.append(b)
print(segregator(lista))

def konwerter(rzymskie):
    liczby_rzymskie = {"I": 1, "V": 5, "X": 10, "L": 50, "C": 100,"D": 500, "M": 1000}
    arabskie = 0
    poprzednia_wartosc = 0
    for symbol in reversed(rzymskie):
        aktualna_wartosc = liczby_rzymskie[symbol]
        if aktualna_wartosc < poprzednia_wartosc:
            arabskie -= aktualna_wartosc
        else:
            arabskie += aktualna_wartosc
        poprzednia_wartosc = aktualna_wartosc
    return arabskie

liczby_rzymskie = "DMMVIII"
arabic_number = konwerter(liczby_rzymskie)
print(f"Liczba rzymska {liczby_rzymskie} to {arabic_number} w systemie arabskim.")


def arabic_to_roman(arabic):
    roman_values = [(1000, 'M'), (900, 'CM'), (500, 'D'), (400, 'CD'),(100, 'C'), (90, 'XC'), (50, 'L'), (40, 'XL'),(10, 'X'), (9, 'IX'), (5, 'V'), (4, 'IV'), (1, 'I')]
    roman = ""
    # Przechodzimy po każdej wartości w odwrotnej kolejności (od największej do najmniejszej)
    for value, symbol in roman_values:
        while arabic >= value:
            roman += symbol  # Dodajemy symbol do wyniku
            arabic -= value  # Zmniejszamy arabic o wartość symbolu
    return roman

arabic_number = 1994
roman_number = arabic_to_roman(arabic_number)
print(f"Liczba arabska {arabic_number} to {roman_number} w systemie rzymskim.")

=========================================================================================KLASY======================================================================

class Account:
    def __init__(self, osoba, stan_konta=0):
        self.osoba = osoba
        self.stan_konta = stan_konta

    def wpłata(self, wplata):
        self.stan_konta += wplata
        print(f"{self.osoba} dokonał wpłaty {wplata} zł. Stan konta: {self.stan_konta} zł.")

    def wyplata(self, wyplata):
        if wyplata > self.stan_konta:
            print(f"Brak wystarczających środków na koncie {self.osoba}.")
        else:
            self.stan_konta -= wyplata
            print(f"{self.osoba} wypłacił {wyplata} zł. Stan konta: {self.stan_konta} zł.")

    def przelew(self, kwota, konto_docelowe):
        if kwota > self.stan_konta:
            print(f"Brak wystarczających środków na koncie {self.osoba} do przelewu.")
        else:
            self.stan_konta -= kwota
            konto_docelowe.stan_konta += kwota
            print(f"{self.osoba} przelał {kwota} zł na konto {konto_docelowe.osoba}.")
            print(f"Stan konta {self.osoba}: {self.stan_konta} zł, Stan konta {konto_docelowe.osoba}: {konto_docelowe.stan_konta} zł.")

    def __str__(self):
        return f"Osoba: {self.osoba}, Stan konta: {self.stan_konta} zł"

class PrivatAccount(Account):
    def __init__(self, osoba, stan_konta=0):
        super().__init__(osoba, stan_konta)

    def przelew_wynagrodzenia(self, kwota, konto_docelowe):
        self.przelew(kwota, konto_docelowe)

    def stan_konta(self):
        print(f"Stan konta {self.osoba}: {self.stan_konta} zł")

class FirmAccount(Account):
    def __init__(self, firma, stan_konta=0):
        super().__init__(firma, stan_konta)

    def przelew_do_zus(self, kwota):
        if kwota > self.stan_konta:
            print(f"Brak środków na koncie {self.osoba} do przelewu na ZUS.")
        else:
            self.stan_konta -= kwota
            print(f"Przelew na ZUS z konta {self.osoba}. Kwota: {kwota} zł.")
            print(f"Stan konta po przelewie: {self.stan_konta} zł.")

    def przelew_do_us(self, kwota):
        if kwota > self.stan_konta:
            print(f"Brak środków na koncie {self.osoba} do przelewu na US.")
        else:
            self.stan_konta -= kwota
            print(f"Przelew podatku do US z konta {self.osoba}. Kwota: {kwota} zł.")
            print(f"Stan konta po przelewie: {self.stan_konta} zł.")

# Przykład użycia klasy FirmAccount
firma1 = FirmAccount("Firma X", 10000)
firma2 = FirmAccount("Firma Y", 5000)

firma1.przelew_do_zus(2000)
firma2.przelew_do_us(1500)
print(firma1)
print(firma2)




class Vector:
    def __init__(self, wektor):
        self.wektor = wektor

    def __add__(self, other):
        if len(self.wektor) != len(other.wektor):
            raise ValueError("Wektory muszą mieć taką samą długość.")
        else:
            return Vector([x + y for x, y in zip(self.wektor, other.wektor)])

    def __sub__(self, other):
        if len(self.wektor) != len(other.wektor):
            raise ValueError("Wektory muszą mieć taką samą długość.")
        else:
            return Vector([x - y for x, y in zip(self.wektor, other.wektor)])

    def __mul__(self, liczba):
        return Vector([x * liczba for x in self.wektor])

    def __str__(self):
        return f"Vector({self.wektor})"

v1 = Vector([1, 2, 3])
v2 = Vector([4, 5, 6])
print(v1 + v2)
print(v1 - v2)
print(v1 * 2)

class Polynomial(Vector):
    def __str__(self):
        # Reprezentacja wielomianu
        terms = []
        for i, coef in enumerate(self.wektor):
            if coef == 0:
                continue
            if i == 0:
                terms.append(f"{coef}")
            elif i == 1:
                terms.append(f"{coef}x")
            else:
                terms.append(f"{coef}x^{i}")
        return " + ".join(terms[::-1]).replace("+ -", "- ")

    def degree(self):
        # Zwraca stopień wielomianu
        for i in range(len(self.wektor) - 1, -1, -1):
            if self.wektor[i] != 0:
                return i
        return 0

    def __getitem__(self, index):
        # Pozwala na odczyt współczynnika przy x^index
        if index < len(self.wektor):
            return self.wektor[index]
        return 0

    def __setitem__(self, index, value):
        # Ustawia współczynnik przy x^index
        if index >= len(self.wektor):
            self.wektor.extend([0] * (index - len(self.wektor) + 1))
        self.wektor[index] = value

    def __add__(self, other):
        # Dodawanie wielomianów
        max_len = max(len(self.wektor), len(other.wektor))
        result = [self[i] + other[i] for i in range(max_len)]
        return Polynomial(result)

    def __sub__(self, other):
        # Odejmowanie wielomianów
        max_len = max(len(self.wektor), len(other.wektor))
        result = [self[i] - other[i] for i in range(max_len)]
        return Polynomial(result)

    def __mul__(self, other):
        # Mnożenie wielomianów
        if not isinstance(other, Polynomial):
            raise ValueError("Można mnożyć tylko dwa wielomiany.")
        result_degree = len(self.wektor) + len(other.wektor) - 1
        result = [0] * result_degree
        for i, coef1 in enumerate(self.wektor):
            for j, coef2 in enumerate(other.wektor):
                result[i + j] += coef1 * coef2
        return Polynomial(result)

    def evaluate(self, x):
        return sum(coef * (x ** i) for i, coef in enumerate(self.wektor))


p1 = Polynomial([2, -1, 3])  
p2 = Polynomial([1, 4])      
print("Wielomian p1:", p1)
print("Wielomian p2:", p2)
print("p1 + p2:", p1 + p2)  
print("p1 - p2:", p1 - p2)  
print("Stopień p1:", p1.degree())  
print("Współczynnik przy x^2 w p1:", p1[2])
p1[2] = 5
print("Zmodyfikowany p1:", p1)
print("p1 * p2:", p1 * p2) 
print("p1(2):", p1.evaluate(2))  



 
class wojownik:
    def __init__(self, nazwa,zdrowie,sila,punkty_takt):
        self.nazwa = nazwa
        self.zdrowie = zdrowie
        self.sila = int(sila)
        self.punkty_takt = int(punkty_takt)
        self.HP = zdrowie
        self.Boost = False

    def MocAtak(self):
        moc = (self.punkty_takt * self.sila * self.zdrowie) * 0.0002 # * 0.002 - to moj balans, na egzamine usunac
        return moc
    def StrataHP(self,obrazenia):
        self.zdrowie -= obrazenia
        procentHP = (self.zdrowie / self.HP) * 100
        if procentHP < 20 and self.Boost == False:
            print('Zdrowie przeciwnika: ',round(procentHP,2),'%')
            self.Boost = True
            self.zdrowie = self.HP * 1.5
            procentHP = (self.zdrowie / self.HP) * 100
            print("Aktywowano boost wojownika! Zdrowie:", procentHP,'%')
        if self.zdrowie > 0:
            return print('Zdrowie przeciwnika: ',round(procentHP,2),'%')
        elif self.zdrowie < 0:
            return print("Pokonałeś przeciwnika!")
class Lucznik:
    def __init__(self, nazwa,zdrowie,zrecznosc,punkty_takt):
        self.nazwa = nazwa
        self.zdrowie = zdrowie
        self.zrecznosc = int(zrecznosc)
        self.punkty_takt = int(punkty_takt)
        self.HP = zdrowie
    def MocAtak(self):
        moc = (self.punkty_takt * self.zrecznosc * self.zdrowie) * 0.0002 # * 0.002 - to moj balans, na egzamine usunac
        return moc
    def StrataHP(self,obrazenia):
        self.zdrowie -= obrazenia
        procentHP = (self.zdrowie / self.HP) * 100
        if self.zdrowie > 0:
            return print('Zdrowie przeciwnika: ',round(procentHP,2),'%')
        elif self.zdrowie < 0:
            return print("Pokonałeś przeciwnika!")
Start = False
Wybor_klasy = input("wybierz klase 'wojownik' lub 'lucznik': ")
if Wybor_klasy == 'wojownik':
    Start = True
    Postac = wojownik('Lukasz', 225, 35, 15)
    Postac2 = Lucznik('Marcel', 100, 75, 25)
elif Wybor_klasy == 'lucznik':
    Postac = Lucznik('Marcel', 100, 75, 25)
    Postac2 = wojownik('Lukasz', 135, 35, 25)
    Start = True
if Start == True:
    print("Kliknij przycisk 'k' zeby zaatakowac przeciwnika")
    while Postac2.zdrowie > 0:
        atak = input()
        if atak == 'k':
            Postac2.StrataHP(Postac.MocAtak())

==============================================================OTWIERANIE PLIKÓW TXT=========================================================

plik = open("test.txt", "a")
if plik.writable():
    ile = plik.write(input("Wprowadź tekst: ") + "\n")
    print("zapisano: ", ile)
plik.close()

plik = open("test.txt", "r")

if plik.readable():
    for l in plik:
        print(l)
    # print(tekst)
    # for l in tekst:
    #     print(l)



import random

plik1 = open("even.txt","a+")
plik2 = open("odd.txt", "a+")
def liczby():
    for i in range(100):
        a = random.randint(-100,100)
        if a % 2 == 0:
            plik1.write(str(a) + ", ")
        else:
            plik2.write(str(a) + ", ")
liczby()
plik1.close()
plik2.close()

plik1 = open("even.txt","r")
plik2 = open("odd.txt", "r")

print("Zawartość pliku even.txt:")
print(plik1.read())

print("Zawartość pliku odd.txt:")
print(plik2.read())

plik1.close()
plik2.close()

# Otwieramy plik do odczytu
with open("even.txt", "r") as plik:
    linia = plik.read().strip()  # Odczytujemy całą linię
    # Dzielimy po przecinkach, usuwamy puste elementy i konwertujemy na int
    liczby1 = [int(x) for x in linia.split(",") if x.strip() != '']  # Dodane sprawdzenie na pusty ciąg

with open("odd.txt", "r") as plik:
    linia = plik.read().strip()  # Odczytujemy całą linię
    # Dzielimy po przecinkach, usuwamy puste elementy i konwertujemy na int
    liczby2 = [int(x) for x in linia.split(",") if x.strip() != '']  # Dodane sprawdzenie na pusty ciąg

# Obliczamy sumę
suma1 = sum(liczby1)
suma2 = sum(liczby2)

# Obliczamy średnią arytmetyczną (jeśli lista nie jest pusta)
if liczby1:
    srednia1 = suma1 / len(liczby1)
else:
    srednia1 = 0  # Jeśli lista jest pusta, średnia wynosi 0

if liczby2:
    srednia2 = suma2 / len(liczby2)
else:
    srednia2 = 0  # Jeśli lista jest pusta, średnia wynosi 0

# Wyświetlamy wyniki
print(f"Suma liczb: {suma1}")
print(f"Średnia arytmetyczna: {srednia1}")
print("\n")
print(f"Suma liczb: {suma2}")
print(f"Średnia arytmetyczna: {srednia2}")

