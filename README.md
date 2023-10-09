# R/Python-Statistics
This will only contain a readme file

# R
2 + 3
# Daje rezultat:
5

# Python
Print(2+3)
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
