# R/Python-Statistics
This will only contain a readme file
## Prvo predavanje

# R
2 + 3
# Daje rezultat:
5

# Python
print(2+3)
# Daje rezultat:
5

# R
sin(0.5)^2+ cos(0.5)^2
# Daje rezultat: 
1

# Python
import math
rezultat = math.sin(0.5)**2 + math.cos(0.5)**2
print(rezultat)
# Daje rezultat: 
1

# R
exp(-Inf)
# Daje rezultat:
0

# Python
import math

rezultat = math.exp(-float('inf'))
print(rezultat)
# Daje rezultat: 
0.0

# R
print(pi, digits=10)
# Daje rezultat:
3.141592654

# Python
import math

pi = math.pi
pi_precision_ten = format(pi, '.10f')
print(pi_precision_ten)
# Daje rezultat:
3.141592654

# R
x<-pi+1 
print(x)
# Daje rezultat: 
4.141593

# Python
import math

x = math.pi + 1
print(x)
# Daje rezultat
4.141592653589793

# R
num1<-2
num2<-2.5
kompl<-num1+2i

# Python
num1 = 2
num2 = 2.5
kompl = num1 + 2j

# R
Kojeg su osnovnog tipa gore definirane varijable ispitujemo funkcijom mode(). Dobijemo 
mode(num1);
mode(num2);
mode(kompl);

# Python 
Kojeg su osnovnog tipa gore definirane varijable ispitujemo funkcijom type()
print(type(num1))
print(type(num2))
print(type(kompl))

# R
rijec<-"abc"

print(rijec);

mode(rijec)

# Python
rijec = "abc"

print(rijec) 

print(type(rijec)) 

# R
num1<-2
num2<-2.5
mode(num1>num2) //logical
num1 > num2   //false

# Python
num1 = 2
num2 = 2.5

rezultat = num1 > num2

print(type(rezultat)) # bool
print(rezultat) # false

# R
log1 <- T
log2 <- TRUE
log3 <- F

mode(log1)  ## [1] "logical"
mode(log2)  ## [1] "logical"
mode(log3)  ## [1] "logical"

# Python
log1 = True
log2 = True
log3 = False

print(type(log1))  # <class 'bool'>
print(type(log2))  # <class 'bool'>
print(type(log3))  # <class 'bool'>

# R
print(log1 + log2)  # [1] 2

print(log1 | log3)  # [1] TRUE
print(log1 & log3)  # [1] FALSE
print(!log1)  # [1] FALSE

# Python
log1 = True
log2 = True
log3 = False

print(log1 + log2)  # Output: 2

# Logičko ILI
print(log1 or log3)  # Output: True

# Logičko I
print(log1 and log3)  # Output: False

# Logička negacija
print(not log1)  # Output: False

# R
Uočimo da je duljina svih varijabli koje smo do sada susreli jednaka 1, što se lagano provjeri funkcijom length(). Varijable, i općenito objekti, čija je duljina veća od 1, mogu se dobiti na različite načine, a jedan od najpopularnijih je korištenje funkcije c u R-u. Njome dobivamo vektore. Na primjer,

vekt <- c(num1, num2)
mode(vekt)   # [1] "numeric"
length(vekt) # [1] 2

Vrijednost varijable vekt je dvodimenzionalni numerički vektor s elementima 2 i 2.5. R će nam to predstaviti kao:

# [1] 2.0 2.5

# Python
U Pythonu korisstimo liste za kreiranje varijabli čija je duljina veća od 2. Možemo definirati listu pomoću uglatih zagrada
num1 = 2
num2 = 2.5

li = [num1, num2]
print(li)  # [2, 2.5]

# R
Vektori su samo jedan od tipova podataka, mogli bi reći i struktura podataka, u R-u. Njihovmode(osnovnitip) može biti bilo koji od prije navedenih osnovnih tipova podataka, a isti je slučaj i s poljima (array) imatricama (matrix). U slučaju ta tri tipa podataka treba uočiti da se oni mogu sastojati samo od istogosnosvnog tipa podataka (dakle, ili samonumericili samocharacteritd.), dok su tipovi podataka kojipodržavaju mješovite osnovne tipove podataka liste (list) idata frame. 

# Python
**Python Tipovi Podataka i Strukture Podataka**

Python podržava različite tipove podataka i strukture podataka koje omogućavaju organizaciju i pohranu podataka. Svaki tip podataka u Pythonu odgovara određenom načinu interpretacije i manipulacije vrijednostima.

1. **Brojevi (Numbers):** Python podržava različite vrste brojeva, uključujući cjelobrojne brojeve (`int`) i brojeve s pomičnim zarezom (`float`). Na primjer:

   integer_num = 42
   float_num = 3.14

2. **Liste (Lists):** Liste su osnovna struktura podataka koja može sadržavati elemente različitih tipova. Ovo je ekvivalent vektorima u R-u. Na primjer:
lista_svega = [1, R, 2, 3, 'Python', 4.5, 'miksvegapomalo']

3. **Nizovi (Arrays):** NumPy, popularna Python biblioteka, omogućava rad s višedimenzionalnim nizovima koji sadrže elemente istog tipa, poput brojeva. Nizovi su učinkoviti za numeričke operacije.

4. **Stringovi**: Stringovi su nizovi znakova koje koristimo za pohranu teksta
    my_string = "Ovo sadrži tekst!"

5. **Rječnici (Dictionaries):** Rječnici su strukture podataka koje omogućavaju pohranu ključeva i njima pridruženih vrijednosti. Svaka vrijednost se može dohvatiti pomoću odgovarajućeg ključa.
dictionary_rj = {'ime': 'Mirko', 'prezime': 'Marić', 'dob': 66}

6. **Skupovi (Sets):** Skupovi su kolekcije jedinstvenih elemenata i koriste se za matematičke operacije nad skupovima
skup = {1, 2, 3, 7, 9}

7. **N-torke (N-tuples):** N-torka je nepromjenjiva (immutable) kolekcija elemenata sa točno određenim brojem elemenata. Nakon što se torka definira, njezini elementi ne mogu se mijenjati.
new_tuple = (1, 'Python', 7, 'R')

8. **Data Frame (Pandas):** Pandas je biblioteka koja omogućava rad s tabličnim podacima u obliku DataFrame-ova, slično radu s podacima u R-ovom Data Frame-u.
import pandas as pd

data = {'grad': ['Pazin', 'Zagreb', 'NN'], 'poštanski_broj': [52000, 10000, 0000]}
df = pd.DataFrame(data)

9. **Mješoviti Tipovi Podataka:**  Slično R-u, u Pythonu možete koristiti liste za pohranu različitih tipova podataka, što omogućava kreiranje mješovitih struktura podataka.
popis_svega = [5, 'Python', 'R', 3.14, {'ime': 'John'}]

## OVO SU PRVE 4 STRANICE PREDAVANJA BROJ 1

# R
# Funkcija c() i vektori
# Kao što smo već napomenuli, osnovne podatke o funkciji c() u R-u možete naći tako da napišete help(c).
# Ukoliko koristite RStudio, u desnom prozoru će vam se otvoriti prozor s opisom funkcije, njezinim argumentima i nekim osnovnim primjerima.

# Ta se funkcija često koristi da se brzo naprave neki vektori tipa:
prviv <- c(2, 2, 2, 2)
drugiv <- c(1:8)

# Elementi tih vektora su, redom:
# [1] 2 2 2 2
# [1] 1 2 3 4 5 6 7 8

# Prvi vektor je duljine 4, dok je drugi duljine 8. Uočimo da smo za vektor drugiv iskoristili mogućnost koju nam pruža R da generiramo sve elemente između niza naredbom `c(1:8)`.

# To se može iskoristiti čak i kada je veći od n. Na primjer:
treciv <- c(8:5)

# Kreira vektor duljine 4, čiji su elementi:
# [1] 8 7 6 5

# R radi s vektorima tako da izvršava operacije ili primjenjuje funkcije po njihovim elementima. Na primjer:
zbrojv <- prviv + treciv
incrv <- drugiv + 1
reciprv <- 1 / prviv

# Elementima vektora se pristupa tako da se nakon imena vektora navede mjesto u vektoru kojem želimo pristupiti u uglatim zagradama. Na primjer, treći element vektora drugiv je broj tri, što možemo dobiti kao:
treci_element <- drugiv[3]

# Uočimo da će R zbrojiti vektore koji nisu jednake duljine tako da reciklira kraći vektor, odnosno da nakon kraja kraćeg vektora započne novi niz elemenata tog vektora. Tako će zbroj vektora drugiv i treciv dati rezultat:
# [1]  9  9  9  9 13 13 13 13

# Mala napomena: vidjeli smo da je jedan način za kreiranje vektora korištenje funkcije c(). Numeričke vektore je moguće stvoriti i korištenjem funkcija rep() i seq(). Funkcija rep() samo ponavlja zadanu vrijednost određeni broj puta. Tako smo vektor prviv mogli napraviti i ovako:
prviv2 <- rep(2, times = 4)

# Ispisuje vektor prviv2: [1] 2 2 2 2

# Funkcija seq() generira niz brojeva od početnog do krajnjeg broja s određenim korakom. Na primjer:
par5 <- seq(2, 10, by = 2)

# Ispisuje vektor par5: [1]  2  4  6  8 10

# Možemo također generirati brojeve između 0 i 1 razmaknute za 0,1:
niz01 <- seq(0, 1, by = 0.1)

# Ispisuje vektor niz01: [1] 0.0 0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9 1.0

# Python
# Funkcija c() i vektori u Pythonu

# U Pythonu koristimo listu za stvaranje vektora. Osnovni podaci o listi i njezinim metodama mogu se pronaći pomoću help(list).

# Prvi vektor
prviv = [2, 2, 2, 2]

# Drugi vektor
drugiv = list(range(1, 9))

# Treći vektor
treciv = list(range(8, 4, -1))

# Operacije s vektorima
zbrojv = [a + b for a, b in zip(prviv, treciv)]
incrv = [x + 1 for x in drugiv]
reciprv = [1 / x for x in prviv]

# R
# Funkcija seq() i vektori

# Kao i kod drugih funkcija, moguće su još neke opcije za funkciju seq(). Na primjer, možemo zadati i koliko vrijednosti želimo da niz sadrži između brojeva. Konkretno, ako želimo između 0 i 9 ubaciti 6 brojeva (uključujući nulu i devetku), možemo upotrijebiti parametar length.out.
niz09 <- seq(0, 9, length.out = 6)
niz09
## [1] 0.0 1.8 3.6 5.4 7.2 9.0

# Naravno, vektori mogu biti i drugog tipa od numeric, a za njihovo kreiranje opet možemo iskoristiti funkciju c() kao što se vidi niže.
ime <- c("Iva", "Ana", "Marko")
ime
## [1] "Iva"   "Ana"   "Marko"

mode(ime)
## [1] "character"

length(ime)
## [1] 3

# Opet, elementima vektora ime pristupamo tako da navedemo u uglatim zagradama element vektora kojem želimo pristupiti. Stoga će nam ime[1] vratiti vrijednost.
ime[1]
## [1] "Iva"

# Pristup elementima vektora nije ograničen samo na navođenje pojedinačnih članova. Naime, može se pristupiti i nekim uzastopnim članovima koristeći već navedenu mogućnost korištenja :.
# Tako možemo dobiti zadnjih četiri elementa vektora drugiv navodeći drugiv[5:8], što rezultira
drugiv[5:8]
## [1] 5 6 7 8

# Korištenjem funkcije c() može se pristupiti, na primjer, samo trećem i petom elementu vektora drugiv:
print(drugiv[c(3, 5)])
## [1] 3 5

# Uočimo da je u gornjem primjeru poredak važan jer će nam drugiv[c(5, 3)] kao rezultat dati
## [1] 5 3

# Može se koristiti i negativna vrijednost indeksa, što rezultira uklanjanjem elementa vektora čiji smo indeks naveli. Na primjer, ukoliko želimo ukloniti treći član vektora drugiv, navest ćemo drugiv[-3], i kao rezultat ćemo dobiti
## [1] 1 2 4 5 6 7 8

# Ni tu nije kraj s baratanjem elemenata vektora (a zapravo i drugih složenijih tipova podataka u R-u). Naime, u R-u je lako izdvojiti sve elemente vektora koji su veći, jednaki, različiti i slični od neke vrijednosti. Na primjer, sve elemente vektora treciv koji su veći ili jednaki od 6 dobivamo tako da u uglatim zagradama navedemo uvjet treciv > 6. Dobivamo treciv[treciv >= 6]:
treciv[treciv >= 6]
## [1] 8 7 6

# Python
# Funkcija seq() i vektori u Pythonu

# U Pythonu možemo koristiti funkciju `numpy.linspace` za postizanje istog efekta kao funkcija `seq()` u R-u.
import numpy as np

# Kreiranje vektora od 0 do 9 s 6 brojeva, uključujući nulu i devetku.
niz09 = np.linspace(0, 9, num=6)

# Ispisuje vektor niz09: [0.  1.8 3.6 5.4 7.2 9. ]

# Kreiranje vektora tipa string
ime = ["Iva", "Ana", "Marko"]

# Ispisuje vektor ime: ['Iva', 'Ana', 'Marko']

# Elementima vektora ime pristupa se isto kao u R-u
prvi_element = ime[0]  # Prvi element vektora

# Ispisuje prvi element: 'Iva'

# Pristup uzastopnim elementima vektora
uzastopni_elementi = ime[1:2]  # Prvi i drugi element vektora

# Ispisuje uzastopne elemente: ['Ana']

# Pristup određenim elementima vektora koristeći listu indeksa
odabrani_elementi = [ime[2], ime[0]]  # Treći i prvi element vektora

# Ispisuje odabrane elemente: ['Marko', 'Iva']

# Uklanjanje elementa iz vektora koristeći negativni indeks
vektor_bez_elementa = ime[-2]  # Bez drugog elementa vektora

# Ispisuje vektor bez elementa: ['Iva', 'Marko']

# Filtriranje elemenata vektora koji ispunjavaju određeni uvjet
veci_od_sest = [x for x in treciv if x >= 6]  # Svi elementi vektora treciv veći ili jednaki 6

# Ispisuje elemente veće ili jednake 6: [8, 7, 6]
# Pristup elementima vektora
treci_element = drugiv[2]  # Python indeksiranje počinje od 0, pa je treći element indeksiran s 2

# Radi s vektorima koji nisu jednake duljine tako da se reciklira kraći vektor
zbrojv2 = [a + b for a, b in zip(drugiv, treciv * (len(drugiv) // len(treciv)) + treciv[:len(drugiv) % len(treciv)])]

# Funkcija rep() u Pythonu nije potrebna jer možemo jednostavno množiti listu s brojem ponavljanja.
prviv2 = [2] * 4

# Funkcija range() u Pythonu je ekvivalent funkciji seq() u R-u
par5 = list(range(2, 11, 2))

# Generiranje brojeva između 0 i 1 s određenim korakom
niz01 = [i / 10 for i in range(11)]

# Ispis rezultata
print("Prvi vektor:", prviv)
print("Drugi vektor:", drugiv)
print("Treći vektor:", treciv)
print("Zbroj vektora prviv i treciv:", zbrojv)
print("Inkrementirani drugi vektor:", incrv)
print("Recipročni prviv:", reciprv)
print("Treći element drugog vektora:", treci_element)
print("Zbroj vektora drugiv i treciv:", zbrojv2)
print("Prvi vektor pomnožen sa 4:", prviv2)
print("Paran brojevi od 2 do 10:", par5)
print("Niz brojeva od 0 do 1 s korakom 0.1:", niz01)

# R
To nije naročito korisno kod malih vektora, ali je jasno da je kod velikih vektora, ili drugih struktura podataka,korisno na brz način izdvojiti elelmente koji zadovoljavaju neki uvjet. 
Naravno, moguće je odrediti na kojim semjestima unutar vektora nalaze elementi koji zadovoljavaju određeni uvjet i to korištenjem funkcije which().
Tako ćemo saznati na kojim se mjestima vektora treciv nalaze elementi koji su veći ili jednaki od 6 na sljedeći način 
which(treciv>=6)
## [1] 1 2 3
Funkcija whichima i dvije ekstenzije: 
which.min
which.max 
Tako možemo odrediti najmanji element vektora treciv kao i mjesto na kojem se element s najmanjom vrijednosti nalazi, odnosno njegov indeks:
min(treciv)
## [1] 5
which.min(treciv)
## [1] 4
Kombinacijom pristupa elementima vektora te korištenjem funkcije which možemo odrediti, na primjer, kojisu sve elementi vektora ime različiti od imena Iva te koji je indeks (na kojem se mjestu nalazi) element vektora ime koji sadrži ime Marko. Imamo ime[ime!="Iva"]
## [1] "Ana"   "Marko" which(ime=="Marko")
## [1] 
3 Vrijedi još napomenuti da se elementima vektora mogu dati i nazivi. Na primjer, elemente vektora ime možemo nazvati prvi, drugi i treći na sljedeći način: names(ime)=c("prvi", "drugi", "treci")pa se prilikom ispisa elemenata vektora ime dobiva
##    prvi   drugi   treci
##   "Iva"   "Ana" "Marko"
Sada se, primjerice, drugom elementu vektora ime može pristupiti preko njegovog indeksa ime[2]
## drugi 
## "Ana"
ili preko imena 
ime["drugi"]
## drugi
## "Ana" 

# Python
# Python
# To nije naročito korisno kod malih vektora, ali je jasno da je kod velikih vektora, ili drugih struktura podataka, korisno na brz način izdvojiti elemente koji zadovoljavaju neki uvjet.
# Naravno, moguće je odrediti na kojim se mjestima unutar vektora nalaze elementi koji zadovoljavaju određeni uvjet i to korištenjem funkcije "numpy.where()".

import numpy as np

treciv = np.array([8, 7, 6, 5])
ime = ["Iva", "Ana", "Marko"]

# Elementi vektora treciv koji su veći ili jednaki od 6:
rezultat_treciv = np.where(treciv >= 6)
print(rezultat_treciv)
# Output: (array([0, 1, 2]),)

# Najmanji element vektora treciv:
min_element_treciv = np.min(treciv)
print(min_element_treciv)
# Output: 5

# Indeks najmanjeg elementa vektora treciv:
indeks_min_elementa = np.argmin(treciv)
print(indeks_min_elementa)
# Output: 3

# Elementi vektora ime koji su različiti od "Iva":
rezultat_ime = [x for x in ime if x != "Iva"]
print(rezultat_ime)
# Output: ['Ana', 'Marko']

# Indeks (na kojem se mjestu nalazi) elementa vektora ime koji sadrži "Marko":
indeks_marko = ime.index("Marko")
print(indeks_marko)
# Output: 2

# R
Mali zadatak: u R-u se operator koji kao rezultat daje ostatak pri dijeljenju dva cijela broja označava s %%.Kako bismo našli sve elemente vektora drugiv koji su parni?
Rješenje: parni brojevi imju ostatak pri dijeljenju s 2 jednak nuli. Dakle, možemo provjeriti koji od elemenata vektora drugiv imaju ostatak pri dijeljenju s 2 jednak nuli. Dobivamo drugiv[drugiv%% 2==0]
## [1] 2 4 6 8
Na ovom mjestu možemo dati jednu napomenu. Rekli smo da funkcija mode kao vrijednost daje jedan odosnovnih tipova podatka, među kojima je i numeric. Naravno, R razlikuje cjelobrojne od realnih brojeva

# Python
Mali zadatak: u Pythonu se operator koji kao rezultat daje ostatak pri dijeljenju dva cijela broja označava s %. Kako bismo našli sve elemente vektora/liste koji su parni?
# Parni brojevi imaju ostatak pri dijeljenju s 2 jednak nuli. Možemo provjeriti koji od elemenata iz drugiv imaju ostatak pri dijeljenju s 2 jednak nuli.

drugiv = [1, 2, 3, 4, 5, 6, 7, 8]

# Pronalaženje parnih brojeva u vektoru drugiv:
parni_brojevi = [x for x in drugiv if x % 2 == 0]
print(parni_brojevi)
# Output: [2, 4, 6, 8]

# R
# Funkcija typeof kao vrijednost vraća način na koji R pohranjuje određeni objekt. Ukoliko se iza broja stavi L, R će taj broj prepoznati kao cjelobrojni. Tako za varijable cjel <- 42L i real <- 12.65 možemo lagano provjeriti da je njihov mode zapravo numeric, ali je typeof(cjel) "integer", a typeof(real) "double".

cjel <- 42L
real <- 12.65

# Provjera tipova varijabli
typeof(cjel)  # Output: "integer"
typeof(real)  # Output: "double"

# Drugi način da se broj pohrani kao cjelobrojni je da se koristi funkcija as.integer. Tako imamo
cjel2 <- as.integer(12)
typeof(cjel2)  # Output: "integer"

# Bez želje za zbunjivanjem napomenut ćemo da u R-u postoji i funkcija class() koja je fleksibilnija od funkcije mode.
# Važna karakteristika R-a, o kojoj nećemo ovdje govoriti, je da korisnik sam može definirati vrijednost funkcije class.

# Python
# U Pythonu, tipovi varijabli se automatski određuju, ali možemo koristiti funkcije za provjeru tipova.

# Definiranje varijabli
cjel = 42
real = 12.65

# Provjera tipova varijabli
tip_cjel = type(cjel)
tip_real = type(real)

# Ispis tipova varijabli
print(tip_cjel)  # Output: <class 'int'>
print(tip_real)  # Output: <class 'float'>

# Drugi način da se broj pohrani kao cjelobrojni u Pythonu je da se koristi funkcija int().
cjel2 = int(12)

# Provjera tipa cjelobrojne varijable
tip_cjel2 = type(cjel2)
print(tip_cjel2)  # Output: <class 'int'>

# U Pythonu također možete koristiti funkciju type() za provjeru tipa objekta.
# Bez želje za zbunjivanjem, napomenut ćemo da Python također podržava razne metode za manipulaciju tipovima podataka, ali o tome se može govoriti detaljnije u drugom kontekstu.

# R
# Matrice
Matrice u R-u tipično možemo kreirati funkcijom matrix, kao što je navedeno u donjem primjeru:

A <- matrix(c(1:6), nrow=2, ncol=3, byrow=TRUE)

Tako dobijemo matricu:

##      [,1] [,2] [,3]
## [1,]    1    2    3
## [2,]    4    5    6

Argumenti funkcije matrix su nrow, odnosno broj redaka i ncol, odnosno broj stupaca te, jasno, sami elementi matrice (u ovom slučaju brojevi od 1 do 6). U gornjem primjeru je definirano byrow=TRUE, što znači da se matrica "puni" po recima. Ukoliko izostavimo taj argument, R će koristiti predefiniranu vrijednost byrow=FALSE, što će uzrokovati "punjenje" matrice po stupcima. U tom slučaju dobivamo matricu:

##      [,1] [,2] [,3]
## [1,]    1    3    5
## [2,]    2    4    6

S obzirom da su matrice dvodimenzionalni objekti, njihovim elementima pristupamo tako da navedemo u uglatim zagradama mjesto u retku i stupcu na kojem se element nalazi. Tako ćemo dobiti da se na trećem mjestu u prvom retku nalazi element 3 jer je:

A[1,3]

## [1] 3

Uočimo da možemo pristupiti i cijelom prvom retku:

A[1,]

## [1] 1 2 3

ili cijelom trećem stupcu:

A[,3]

## [1] 3 6

Kao i kod vektora, možemo pristupati elementima matrice i na složenije načine. Tako drugi i treći stupac možemo izdvojiti s:

A[,c(2,3)]

i dobiti:

##      [,1] [,2]
## [1,]    2    3
## [2,]    5    6

ili pak možemo izdvojiti sve elemente matrice A koji su veći ili jednaki od 3:

A[A >= 3]

## [1] 4 5 3 6

Kada primijenimo funkciju mode na varijablu A, dobit ćemo vrijednost numeric. S druge strane, imamo:

typeof(A)

## [1] "integer"

class(A)

## [1] "matrix" "array"

## Python
import numpy as np

# Kreiranje matrice
A = np.array([[1, 2, 3],
              [4, 5, 6]])

# Pristup elementima matrice
element = A[0, 2]  # Pristup elementu u prvom retku i trećem stupcu (indeksi se broje od 0)
print(element)  # Output: 3

# Pristup cijelom retku ili stupcu
prvi_redak = A[0, :]  # Pristup cijelom prvom retku
treci_stupac = A[:, 2]  # Pristup cijelom trećem stupcu
print(prvi_redak)  # Output: [1 2 3]
print(treci_stupac)  # Output: [3 6]

# Izdvajanje elemenata koji zadovoljavaju uvjet
uvjet = A >= 3
rezultat = A[uvjet]  # Izdvajanje elemenata većih ili jednakih 3
print(rezultat)  # Output: [3 4 5 6]

# Provjera tipa podataka
tip = A.dtype  # Tip podataka u matrici
print(tip)  # Output: int64

# R
# Matrice
Matrice u R-u tipično možemo kreirati funkcijom matrix, kao što je navedeno u donjem primjeru:

A <- matrix(c(1:6), nrow=2, ncol=3, byrow=TRUE)

Tako dobijemo matricu:

##      [,1] [,2] [,3]
## [1,]    1    2    3
## [2,]    4    5    6

Argumenti funkcije matrix su nrow, odnosno broj redaka i ncol, odnosno broj stupaca te, jasno, sami elementi matrice (u ovom slučaju brojevi od 1 do 6). U gornjem primjeru je definirano byrow=TRUE, što znači da se matrica "puni" po recima. Ukoliko izostavimo taj argument, R će koristiti predefiniranu vrijednost byrow=FALSE, što će uzrokovati "punjenje" matrice po stupcima. U tom slučaju dobivamo matricu:

##      [,1] [,2] [,3]
## [1,]    1    3    5
## [2,]    2    4    6

S obzirom da su matrice dvodimenzionalni objekti, njihovim elementima pristupamo tako da navedemo u uglatim zagradama mjesto u retku i stupcu na kojem se element nalazi. Tako ćemo dobiti da se na trećem mjestu u prvom retku nalazi element 3 jer je:

A[1,3]

## [1] 3

Uočimo da možemo pristupiti i cijelom prvom retku:

A[1,]

## [1] 1 2 3

ili cijelom trećem stupcu:

A[,3]

## [1] 3 6

Kao i kod vektora, možemo pristupati elementima matrice i na složenije načine. Tako drugi i treći stupac možemo izdvojiti s:

A[,c(2,3)]

i dobiti:

##      [,1] [,2]
## [1,]    2    3
## [2,]    5    6

ili pak možemo izdvojiti sve elemente matrice A koji su veći ili jednakih od 3:

A[A >= 3]

## [1] 4 5 3 6

Kada primijenimo funkciju mode na varijablu A, dobit ćemo vrijednost numeric. S druge strane, imamo:

typeof(A)

## [1] "integer"

class(A)

## [1] "matrix" "array"

Možemo uočiti da su matrice zapravo specijalni slučajevi tipa podataka array, koji mogu imati više od dvije dimenzije (dakle, ne samo stupce i retke, nego i dodatne "smjerove"). Kako svaki objekt u R-u, kao što smo rekli na početku, ima duljinu, vidimo da primjenom funkcije length(A) dobivamo vrijednost 6. Jasno, kod matrica je relevantna i dimenzija matrice, u matematičkom smislu, pa možemo provjeriti da je dim(A):

dim(A)

## [1] 2 3

S obzirom da R prioritetno obavlja sve operacije na razini elemenata dodavanjem broja matrici, na primjer, zapravo dodajemo broj svakom elementu matrice. Tako će nam operacija A + 2 rezultirati matricom:

##      [,1] [,2] [,3]
## [1,]    3    4    5
## [2,]    6    7    8

dok će operacija A * 2 dati matricu:

##      [,1] [,2] [,3]
## [1,]    2    4    6
## [2,]    8   10   12

Naravno, R podržava i "obično" množenje matrica pomoću operatora %*%, pa će tako umnožak matrice A i transponirane matrice od A, koju izračunamo pomoću t(A), dati novu matricu koja je jednak produktu te dvije matrice:

##      [,1] [,2]
## [1,]   14   32
## [2,]   32   77

# Python
import numpy as np

# Kreiranje matrice A
A = np.array([[1, 2, 3],
              [4, 5, 6]])

# Pristup elementima matrice
element = A[0, 2]  # Pristup elementu u prvom retku i trećem stupcu (počinje s 0)
print(element)  # Output: 3

# Pristup cijelom retku ili stupcu
prvi_redak = A[0, :]  # Pristup cijelom prvom retku
treci_stupac = A[:, 2]  # Pristup cijelom trećem stupcu
print(prvi_redak)  # Output: [1 2 3]
print(treci_stupac)  # Output: [3 6]

# Pristup elementima koji zadovoljavaju uvjet
uvjetni_elementi = A[A >= 3]  # Elementi veći ili jednaki 3
print(uvjetni_elementi)  # Output: [3 4 5 6]

# Operacije s matricama
rezultat_zbrajanja = A + 2  # Zbrajanje svakog elementa s brojem 2
rezultat_mnozenja = A * 2  # Množenje svakog elementa s brojem 2
print(rezultat_zbrajanja)
# Output:
# [[3 4 5]
#  [6 7 8]]
print(rezultat_mnozenja)
# Output:
# [[ 2  4  6]
#  [ 8 10 12]]

# Umnožak matrice A i transponirane matrice A
umnozak = np.dot(A, A.T)
print(umnozak)
# Output:
# [[14 32]
#  [32 77]]

# R
# Liste
Liste su vrlo općeniti tipovi podataka u R-u koje se mogu sastojati od podataka raznih sastavljenih od osnovnih tipova podataka. Na primjer, uz već prije definirane varijable, definiramo i jednu logičku:
logi <- c(T, T, F, F, T)

pa onda i listu:
lista <- c(treciv, ime, logi)

koju R prikazuje kao:

##                                    prvi   drugi   treci
##     "8"     "7"     "6"     "5"   "Iva"   "Ana" "Marko"
##  "TRUE"  "TRUE" "FALSE" "FALSE"  "TRUE"

Ukoliko želimo maknuti nazive vektora ime dovoljno je izvršiti naredbu:
names(lista) <- c()

da dobijemo:

##  [1] "8"     "7"     "6"     "5"     "Iva"   "Ana"   "Marko" "TRUE"  "TRUE"
## [10] "FALSE" "FALSE" "TRUE"

Liste su u osnovi liste vektora (vektor vektora) različite duljine. Ukoliko definiramo listu u kojoj svi vektori imaju istu duljinu dobivamo data frame-ove kojima ćemo uglavnom raditi. Data frame-ovi se zapravo koriste za pohranu tabličnih podataka. Kao primjer možemo uzeti već postojeći vektor ime, ukloniti nazive elemenata i napraviti novi:
dob <- c(21, 25, 22)

te definirati data frame:
names(ime) <- c()
pod <- data.frame(ime, dob)

Tako dobivamo:

##     ime dob
## 1   Iva  21
## 2   Ana  25
## 3 Marko  22

Varijabla pod je tipa data frame, a R je u osnovi tretira kao listu što vidimo pomoću:
class(pod)

## [1] "data.frame"

typeof(pod)

## [1] "list"

Možemo uočiti da nam gornji podaci nisu previše informativni, ali zato možemo iskoristiti funkciju str() koja će dati detaljniji opis interne strukture objekata u R-u pa tako i našeg pod. Imamo:

str(pod)

## 'data.frame':    3 obs. of  2 variables:
##  $ ime: chr  "Iva" "Ana" "Marko"
##  $ dob: num  21 25 22

Data frame-ove možemo lagano proširivati. Tako u pod možemo dodati i visinu svake od osoba čija su imena navedena u vektoru ime:
vis <- c(165, 172, 180)

te dobiti:

pod <- data.frame(pod, vis)

pod

##     ime dob vis
## 1   Iva  21 165
## 2   Ana  25 172
## 3 Marko  22 180

Pomoću str() možemo provjeriti novu strukturu tako dobivenog data frame-a:

str(pod)

## 'data.frame':    3 obs. of  3 variables:
##  $ ime: chr  "Iva" "Ana" "Marko"
##  $ dob: num  21 25 22
##  $ vis: num  165 172 180

Vratit ćemo se kasnije data frame-ovima, a za sada ćemo završiti s ovim pregledom tipova podataka u R-u.

# Python
# Liste
# U Pythonu koristimo liste za sličnu funkcionalnost kao liste u R-u.
logi = [True, True, False, False, True]

# Možemo stvoriti listu koja sadrži različite tipove podataka.
lista = [treciv, ime, logi]

# Da bismo uklonili nazive iz vektora ime, možemo koristiti "_".
ime = []

# Prikaz liste
print(lista)

# Data frame-ovi u Pythonu obično se stvaraju pomoću pandas biblioteke.
import pandas as pd

# Stvaranje data frame-a
dob = [21, 25, 22]
df = pd.DataFrame({'ime': ime, 'dob': dob})

# Prikaz data frame-a
print(df)

# Dodavanje novog stupca u data frame
vis = [165, 172, 180]
df['vis'] = vis

# Prikaz proširenog data frame-a
print(df)

# R
# Učitavanje i snimanje podataka u R-u
# R učitava i snima podatke (datoteke) u tzv. radnom direktoriju (working directory). 
# Ukoliko niste sigurni koji je trenutno definiran radni direktorij, 
# to možete provjeriti funkcijom getwd(), dok promjenu radnog direktorija obavljamo funkcijom setwd().

# Primjer promjene radnog direktorija
setwd("C:/Sveuciliste-Pula/Statistika/Markdown/Predavanja")

# Prikaz trenutnog radnog direktorija
getwd()

# Učitavanje Excel datoteke
# Za učitavanje Excel datoteka u R-u možemo koristiti funkciju read.xlsx iz odgovarajućih paketa.
# Prvo trebamo instalirati i učitati potrebne pakete.
library("rJava")
library("xlsx")
library("xlsxjars")

# Učitavanje Excel datoteke "BMI.xlsx" iz lista "Prva" u data frame "podaci"
podaci <- read.xlsx("BMI.xlsx", sheetName = "Prva", header = TRUE, endRow = 13)

# Prikaz strukture podataka
str(podaci)

# Prikaz podataka
podaci

# Pristupanje podacima u data frame-u
# Na primjer, podatke o visini dobijemo na sljedeći način
visina <- podaci$Visina

# Filtriranje podataka
# Primjer filtriranja osoba manje ili jednako 180 cm po visini
niska_visina <- podaci$Visina[podaci$Visina <= 180]

# Izračun BMI
# Računanje BMI-ja i dodavanje rezultata u data frame
BMI <- podaci$Tezina / ((podaci$Visina / 100) ^ 2)
podaci <- data.frame(podaci, BMI)

# Snimanje podataka u Excel datoteku "BMI2.xlsx"
write.xlsx(podaci, "BMI2.xlsx", sheetName = "Druga", col.names = TRUE)
Mogli smo podatke snimiti i u prvi file BMI, ali postoji mogućnost da bi “pregazili” prethodno postojećepodatke pa smo prikazali način da se podaci snime u jednu drugu Excel tablicu (koju smo prije toga kreirali).Naravno, R može čitati i razne druge formate datoteka, poput.csvi to funkcijomread.csv, ali i HTMLtablice. Učitavanje podataka u raznim formatima je tema za sebe, a nama će biti dovoljne osnovne funkcijekako bismo učitali podatke koji će nam trebati.

# Python
import os
import pandas as pd

# Promjena radnog direktorija
os.chdir("C:/Sveuciliste-Pula/Statistika/Markdown/Predavanja")

# Prikaz trenutnog radnog direktorija
print(os.getcwd())

# Učitavanje Excel datoteke
# Koristimo pandas library za rad s Excel datotekama
podaci = pd.read_excel("BMI.xlsx", sheet_name="Prva", header=0, nrows=13)

# Prikaz strukture podataka
print(podaci.info())

# Prikaz podataka
print(podaci)

# Pristupanje podacima u DataFrame-u
# Na primjer, podatke o visini dobijemo na sljedeći način
visina = podaci["Visina"]

# Filtriranje podataka
# Primjer filtriranja osoba manje ili jednako 180 cm po visini
niska_visina = podaci[podaci["Visina"] <= 180]

# Izračun BMI
# Računanje BMI-ja i dodavanje rezultata u DataFrame
podaci["BMI"] = podaci["Tezina"] / ((podaci["Visina"] / 100) ** 2)

# Snimanje podataka u Excel datoteku "BMI2.xlsx"
podaci.to_excel("BMI2.xlsx", sheet_name="Druga", index=False)
