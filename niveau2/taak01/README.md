# PHP-EXPERT-NIVEAU2-Taak01

## OOP - Object Oriented Programming

In deze opdracht ga je kennis maken met een belangrijk concept binnen programmeren: OOP.
OOP staat voor Object Oriented Programming. De meeste software ontwikkelaars werken hiermee. Het is een manier om code te ordenen. Je hebt er al eens gebruik van gemaakt zonder dat je het wist.

### Objecten in de echte wereld

### Uitleg 1: objecten

De wereld om je heen bestaat uit objecten. Denk maar aan de muis in je hand, of het bureau waar je aan zit. Maar ook jij als mens kan je definieren als object.
Daarnaast zijn huizen, auto's, speeltuinen en voetbalveldjes ook objecten. Eigenlijk is alles een object, als we het puur vanuit een software ontwikkelaar kijken.

> ##### Regel 1: Alles is een object

### Uitleg 2: properties (eigenschappen)

Alle eerder genoemde objecten hebben eigenschappen, zoals kleur, grootte, materiaalsoort en titel of naam. Zo heeft een auto een bepaalde kleur, hoogte en merk en type naam.
Andere objecten hebben vaak weer andere _eigenschappen_. Het Engelse woord voor eigenschap is ook wel _property_.

> ##### Regel 2: Elk object heeft een of meer eigenschappen

### Uitleg 3: methods (functionaliteiten)

Alle eerder genoemde objecten hebben naast eigenschappen ook _methods_. Dit betekent simpelweg dat objeten dingen kunnen **doen!**. Een aantal voorbeelden

- een auto: kan starten, kan rijden, kan stoppen en kan keren
- een mens: kan lopen, kan springen, kan tekenen, kan programmeren.
- een speeltuin kan opengaan, dichtgaan.

Methods zijn functionaliteiten (functions) van een object.

> ##### Regel 3: Elk object heeft een of meer methods/functions

### Objecten in PHP

Binnen programmeertalen zijn er ook objecten. Vaak krijg je die van de bedenkers van de taal aangeleverd. Maar soms of soms vaak, moet je zelf objecten bedenken. En om dit te doen moet je eerst een blauwdruk maken, een tekening van het object voordat je het object maakt. Je maakt toch ook nooit een huis zonder bouwtekening of nooit een game of website zonder eerst een plan te maken.

Bij programmeren maken we altijd eerst een tekening om daarna een object te maken. Zo'n _tekening_ noemmen we een **class**. Als we een class van een student willen maken dan ziet dat er zo uit

```php
class Student(){

}
```

Willen we properties toevoegen aan de student bouwtekening dan kunnen we dat zo doen:

```php
class Student(){
  $voornaam;
  $achternaam;
  $leeftijd;
  $studentnummer;
}
```

#### Van Class naar Object

Ok, je hebt nu een mooie bouwtekening gemaakt. Deze **class** gaan we omzetten in een **object**

```php
class Student(){
  $voornaam;
  $achternaam;
  $leeftijd;
  $studentnummer;
}

$nieuweStudent = new Student(); //met het woordje new maken we een nieuw object

$nogEenNieuweStudent = new Student(); //en nu hebben we nog een student gemaakt.
```

## Leerdoelen

> 1. [ ] Ik maak een class
> 2. [ ] Ik maak een van de eerder gemaakte class een object

## Opdracht

> 1. Maak een class _auto_
> 2. Geef de volgende properties aan de auto: merk, kleur, type, uitvoering, brandstof
> 3. Maak van de class een object, ofwel maak een auto-object. Gebruik de variable \$nieuweAuto

## Bronnen

> * [Geek For Geeks - PHP | Classes](https://www.geeksforgeeks.org/php-classes/)
> * [Geek For Geeks - PHP | Objects](https://www.geeksforgeeks.org/php-objects/)
