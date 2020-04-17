# PHP-EXPERT-NIVEAU2-Taak01

## Medewerkers

## Uitleg

In deze opdracht ga je nog meer data uit een database halen met behulp van het PDO object. Maar nu ga je gebruik maken van **prepared statements**. Met prepared statements ofwel _queries die voorbereid zijn_ kun je variabelen toevoegen op een een juiste wijze. Je voorkomt hiermee SQL injecties.

Onthoud: Als je variabelen wilt gebruiken in een query dan moet je **placeholders** gebruiken

Je schrijft een query nu als volgt:

```php
$sql = 'SELECT * FROM users WHERE email = :email AND status= :status;
```

Tijdens deze module gebruiken we dus de combinatie van een **:** en een _woord_ erachter als placeholders.
Dat is het maken van een query. Daarna _prepare_ je de query met behulp van **PDO::prepare()**

```php
$database_connectie->prepare($sql)
```

Je maakt wederom gebruik van het `$statement` object om de query uit te voeren ofwel _execute()_ prepared sql.

```php
$statement->execute([['email' => $email, 'status' => $status]]);
```

De query is uitgevoerd en nu bepaal je wat je wilt doen met de query (aantal gevonden voorwerpen of alle records ophalen, etcetera). In dit geval de gegevens van de gebruiker ophalen:

```php
$user = $statement->fetch();
```

De volledige code:

```php
$sql = 'SELECT * FROM users WHERE email = :email AND status= :status';
$database_connectie->prepare($sql);
$statement->execute([['email' => $email, 'status' => $status]]);
$user = $statement->fetch();
```

## Leerdoelen

> 1. [ ] Ik toon een enkele rij gegevens uit een database tabel met behulp van PDO

## Opdracht

> 1. Maak gebruik van de database `toolsforever`.
> 2. Maak in index.php van deze opdracht een database connectie.
> 3. Haal de gegevens op met een SELECT WHERE statement en haal uit de `gebruikers` tabel alleen de gegeven van _Mohamed Hadid_ op.
> 4. Toon de gegevens op het scherm.

## Eindresultaat

![Eindresultaat](https://github.com/ROC-van-Amsterdam-College-Amstelland/PHP-EXPERT/blob/master/niveau3/taak02/images/resultaat.png)

## Bronnen

> [PHP Delusions - PDO](https://phpdelusions.net/pdo)  
> [Geek For Geeks - Associative Arrays in PHP](https://www.geeksforgeeks.org/associative-arrays-in-php/)