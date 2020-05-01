# PHP-EXPERT-NIVEAU3-Taak03

## Medewerkers

## Uitleg

In deze opdracht ga je nog meer data uit een database halen met behulp van het PDO object. Maar nu ga je gebruik maken van **prepared statements**. Met prepared statements ofwel _queries die voorbereid zijn_ kun je variabelen toevoegen op een een juiste wijze. Je voorkomt hiermee SQL injecties.

Onthoud: Als je variabelen wilt gebruiken in een query dan moet je **placeholders** gebruiken

Je schrijft een query nu als volgt:

```php
$sql = 'SELECT * FROM users WHERE email = :email AND status= :status;
```

Je ziet hierboven twee placeholders staan: `:email` en `:status`
Tijdens deze module gebruiken we dus de combinatie van een **:** en een _woord_ erachter als placeholders.
Dat is het maken van een query. Daarna _prepare_ je de query met behulp van **PDO::prepare()**

```php
$database_connectie->prepare($sql)
```

Je maakt wederom gebruik van het `$statement` object om de query uit te voeren ofwel _execute()_ de sql string die net is voorbereid.

```php
$statement->execute([['email' => $email, 'status' => $status]]);// hier koppel je opgegeven variabelen en de placeholders aan elkaar met een associatieve array
```

De query is uitgevoerd en nu bepaal je wat je wilt doen met de query (aantal gevonden voorwerpen of alle records ophalen, etcetera). In dit geval de gegevens van de gebruiker ophalen:

```php
$user = $statement->fetch(); //haal 1 rij uit de database op met de method fetch()
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
> 3. Haal de gegevens op met een SELECT WHERE statement en haal uit de `gebruikers` tabel alleen de gegevens van _Mohamed Hadid_ op.
> 4. Bij 3 moet je wel gebruik maken van _prepared statements_
> 5. Toon de gegevens op het scherm.

## Eindresultaat



## Bronnen

> [PHP Delusions - PDO](https://phpdelusions.net/pdo)  
> [Geek For Geeks - Associative Arrays in PHP](https://www.geeksforgeeks.org/associative-arrays-in-php/)