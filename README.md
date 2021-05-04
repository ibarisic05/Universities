# Popis sveučilišta u RH
Cilj laboratorijskih vježbi je kreirati mobilnu aplikaciju u kojoj korisnik dohvaća podatke podatke putem `API` poziva i iste prikazuje unutar `UITableView-a`

# Razvoj mobilnih aplikacija - LV 3

Treća po redu laboratorijska vježba iz kolegija Razvoj mobilnih aplikacija kroz koju će se studenti upoznati dohvatom podataka putem `API` poziva, parsanjem odgovora i prikazivanjem dobivenih rezultata unutar `UITableView-a`.

  

Prvi dio vježbe stavlja fokus na dohvat podataka i generiranje `Array-a` objekata koji će se prikazivati u `TableView-u`. Osim što će se studenti susresti  sa vanjskim bibliotekama za dohvat i parsanje podataka, isti će dobiti kratak uvid u rad sa `Thread-ovima`.

  

Drugi dio vježbe je generiranje prikaza podataka u `UITableView-u` i prikazivanje podataka.

  
Za vježbu će se koristiti [Alamofire](https://github.com/Alamofire/Alamofire) library koji će se koristiti za dohvat podataka putem `API` poziva i [SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON) za parsanje odgovora u objekte.

  

## Popis sveučilišta u RH - iOS

## Zadatak 1

- Kreirati novi projekt Popis sveučilišta

- Koristeći Alamofire dohvatiti podatke sa linka (link je `GET` request i na istome nema autorizacije): `http://universities.hipolabs.com/search?country=croatia`

- U odgovoru sa servera, na `Background Thread-u` napraviti provjeru da li je odgovor ispravan ili smo dobili grešku, u slučaju greške istu ispisati

- Kreirati objekt `University` i u istom definirati varijable `name`, `url` i `country`, prilikom inicijalizacije parametara koristeći `SwiftyJSON` dodijeliti varijablama pripadajuću vrijednost.

- Kod ispravnog odgovora napraviti mapiranje podataka u `Array` objekata `University`

- Vratiti mapirane podatke na `Main Thread-u`

## Zadatak 2

- Na inicijalni `UIViewController` dodati `UITableView` i kreirati `UITableViewCell` koji će prikazati popis sveučilišta i na istom popisu za svako sveučilište ispisati `name`, `state` i `url` parametre sveučilišta. 


### Prikaz screen-ova
1. [Popis sveučilišta](https://raw.githubusercontent.com/ibarisic05/MyDestinations/master/photos/lista_destinacija.png)

# Korisni linkovi

-  [Struct and Class](https://docs.swift.org/swift-book/LanguageGuide/ClassesAndStructures.html) - dodatne informacije o klasama i strukturama

-  [UITableView](https://developer.apple.com/documentation/uikit/uitableview) - dokumentacija za UITableView

- [Package Manager](https://swift.org/package-manager/) - detaljan opis Swift Package Managera

- [Alamofire](https://github.com/Alamofire/Alamofire) - library za rad sa `API` requestovima

- [SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON) - library za parsanje `JSON-a`
