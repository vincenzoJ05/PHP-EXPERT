# PHP-EXPERT-NIVEAU1-Taak01

## Studentenoverzicht

## Uitleg

De meeste data die jij uit een database gaat halen bestaan uit arrays. Maar dit zijn niet altijd eenvoudige arrays. Vaak zijn het _multidimensionale_ arrays. Dit betekent dat er een array meerder arrays kan bevatten. Hieronder staat een voorbeelden van drie typen arrays. De eerste twee ken je al:

Numerieke arrays
```
$getallen = [45,6546,676,234,8765];
$namen = ['bart', 'david', 'emiel'];
```
Associatieve arrays
```
$medewerker = [
  'voornaam' => 'Willem',
  'achternaam' => 'van Oranje',
  'functie'  => 'koning'
];

$frisdrank = [
  'naam' => 'Cola',
  'merk' => 'Coca Cola',
  'hoeveelheid'  => '1 liter'
];
```
Multidimensionale array
```
$medewerkers = [
  [
    'voornaam' => 'Willem',
    'achternaam' => 'van Oranje',
    'functie'  => 'koning'
  ],
  [
    'voornaam' => 'Donald',
    'achternaam' => 'Trump',
    'functie'  => 'president'
  ]
];

/* De medewerkers array heeft twee arrays. Een array op index 0 en een array op index 1
 *  Om een enkele waarde op het scherm te tonen doe je bijvoorbeeld dit.
 *
 *   <--medewerker->      
echo $medewerkers[0]['voornaam'] // Willem
echo $medewerkers[1]['voornaam'] // Donald

```


## Leerdoelen

Eén of meerdere leerdoelen die het liefst SMART zijn geformuleerd en slaan op de inhoud van deze taak.  
> Voorbeeld:
>
> 1. [ ] Ik kan met PHP een functie aanspreken

## Opdracht

> 1. Schrijf code in `index.php` met daarin een array genaamd `$studenten`
> 2. Vul deze array met een nog een array dat bestaat uit een associatieve array met de volgende _keys_ __voornaam__, __achternaam__, __leeftijd__

## Eindresultaat

Duidelijk maken hoe het succesvol maken van de taak eruit ziet. Dit kan tekstueel of liever als mogelijk met gebruik van screenshots / filmpjes  
> Voorbeeld:  
> Als je de code uitvoert dan zie je zoiets als dit:



## Bronnen

>[W3 Schools - PHP Arrays](https://www.w3schools.com/php/php_arrays_associative.asp)  
>[Geek For Geeks - Associative Arrays in PHP](https://www.geeksforgeeks.org/associative-arrays-in-php/)  
>[PHP Manual - Arrays](https://www.php.net/manual/en/language.types.array.php)  
