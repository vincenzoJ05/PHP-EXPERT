# PHP-EXPERT-NIVEAU2-Taak05

## OOP - Object Oriented Programming

Een methode gebruiken die met properties aan de haal gaat

### methods

Je kunt natuurlijk ook methods maken die properties aanpassen of de dan geldige waardes ophalen.

### voorbeeld
Zo kun je bijvoorbeeld de _soort_ van een object instellen met een method. Je ziet dat hier het woordje __$this__ wordt gebruikt. Dat komt omdat we bij het maken van de class nog niet weten wat de namen van de objecten zullen zijn. Later weten we dat `$eenHond` gebruikt gaat worden. Maar nu weten we dat eigenlijk nog niet. Maar we willen wel de string `Duitse Herder` toekennen aan de _soort_ propertie. `$this` gaat over _deze_ class (of je kunt ook wel zeggen: gaat over dit object: dit=this)

```php
class Hond{
    $naam;
    $soort;

    function setSoort(){ 
        $this->soort = 'Duitse Herder';
    }
}
```
En hoe gebruik je dan zo'n method (functie) dan? Bekijk eens onderstaand voorbeeld:
```php
$eenHond = new Hond();
$eenHond->naam = 'Bassie';
$eenHond->setSoort();
```
Nu is deze method `setSoort()` niet heel flexibel. Want steeds dezelfde string wordt toegekend. We zouden ook met parameters kunnen werken om de method dynamischer te maken:

```php
class Hond{
    $naam;
    $soort;

    function setSoort($soort_parameter){ 
        $this->soort = $soort_parameter;
    }
}

$eenHond = new Hond();
$eenHond->setSoort('Duitse Herder');
```
In bovenstaand voorbeeld wordt het al een stuk dynamischer. Nogmaals: Niet hele boeiende applicatie.

## Leerdoelen

> 1. [ ] Ik maak een `set`-methode aan die een propertie waarde geeft
> 2. [ ] Ik maak een `get`-methode aan die een propertie ophaalt

## Opdracht

> 1. Maak een class _Lamp_
> 2. Geef de Lamp class de volgende properties: kleur, helderheid, isAan
> 3. Maak twee objecten aan: $woonkamerLamp en $keukenLamp. 
> 4. Geef de properties van de objecten waardes: 
> - $woonkamerLamp: kleur="geel", helderheid="zacht", isAan=true
> - $keukenLamp: kleur="wit", helderheid="vel", isAan=uit
> 5. Maak in de class nu een method aan die de propertie isAan kan wijzigen. Noem deze method `setStatus($status)`
> 6. Maak gebruik van de method `setStatus($status)` om de woonkamerLamp uit te zetten
> 7. Maak in de class nu een method aan die huidige waarde van de propertie isAan kan ophalen. Noem deze method `getStatus()`.  Gebruik return in de method
> 8. Maak gebruik van de method `getStatus()` om de keukenLamp op te halen.



## Bronnen

> * [Geek For Geeks - PHP | Classes](https://www.geeksforgeeks.org/php-classes/)
> * [Geek For Geeks - PHP | Objects](https://www.geeksforgeeks.org/php-objects/)
