# Proiect
## 1.Introducere 

Cinefil(m) este o aplicatie care presupune managementul filemelor favorite. Produsul nostru isi propune sa gestioneze pentru fiecare utilizator in parte preferintele lui in materie cinematografica. Acesta va contine liste pentru filmele favorite sortate in categorii de catre utilizator, el oferind posibilitatea de a cauta noi filme, de a adauga si de a sterge elemente din lista. Pe langa aceste liste, produsul nostru va oferi si posibilitatea afisarii unei statistici legate de genul cel mai indragit de catre utilizator, prezentand un top al categoriilor din care fac parte majoritatea filmelor favorite. Aplicatia integreaza TMDB (The Movie Database) luand informatiile legate de filme de pe aceast site. Proiectul, o aplicatie web, creata cu ajutorul tehnologiilor web HTML5, JavaScript va prezenta informatii furnizate de [TMDB](https://www.themoviedb.org/). 

Produsul nostru se adreseaza, in special, cinefililor de toate varstele, fiind usor de utilizat si eficient in gestionarea preferintelor cinematografice. Consideram ca exista foarte multe persoane doritoare sa gaseasca un manager de filme care sa le serveasca in a usura sarcina de a inregistra de mana filmele pe care le-au vazut si detaliile aferente lor. 

Cinefil(m) intra in competitie cu aplicatii precum [My Movies](https://www.mymovies.dk/), [Letterboxd](https://letterboxd.com/) si popularul [IMDb](https://www.imdb.com/)  (Internet Movie Database). My Movies este o aplicatie platita, atat pentru desktop, cat si pentru dispozitivele mobile. Aceasta ii permite utilizatorului sa vizioneze filmele din colectia sa. Letterboxd isi doreste sa fie vazut mai mult ca un jurnal de filme, unde persoanele interesate pot sa dea note filmelor si sa comunice cu alte persoane in functie de gusturile lor in materie cinematografica.

## 2.Interfețe aplicație
![alt text](https://github.com/AMarines02/Proiect/blob/master/1.jpg)

![alt text](https://github.com/AMarines02/Proiect/blob/master/3.jpg)

![alt text](https://github.com/AMarines02/Proiect/blob/master/2.jpg)

![alt text](https://github.com/AMarines02/Proiect/blob/master/5.jpg)

## 3.API REST
1.Vezi genurile de filme
get /genre
[ {
	"gen":"Comedie",
	"numarFilme":"375"
   }
]
2. Vezi filmele dintr-un anumit gen(id)
get/genre/:id/movies
3.Cautarea unui film
get/movies/?:search=
[
  {
	"titlu":"Dead and loving it"
	"director":"Mel Brooks",
	"an":"1995",
        "durata":"88"
   }
]
4.Adaugarea unui film
get/movies/?search=
put/favorite/:id
5.Stergerea unui film din lista de favorite
get/movies/?search=
delete/favorite/:id



