# PHP-EXPERT Moduleopdracht

## Voetbalclub ASD `20

## Toelichting

De voetbalclub moet een administratiesysteem hebben van wie in welk team speelt maar ook of het lid betaald heeft of niet. Kortom een administratiesysteem voor leden. Daarnaast wil de club ook verschillende totaaloverzichten kunnen maken van de verschillende teams.

## Leerdoelen

> 1. [ ] Ik maak een applicatie om de leden administratie van de voetbalclub te kunnen beheren

## Opdracht

> - Je mag gebruik maken van een CSS framework
>
> ##### Database
> 
> 1. [ ] Maak een database: `voetbalclubASD`

> ##### Gebruikers
> 
> 2. [ ] Maak een database tabel: `gebruikers`
> 3. [ ] Maak de volgende _kolommen_ aan:
>       - id (int:11)
>       - voornaam (varchar:100)
>       - achternaam (varchar:100)
>       - email (varchar:200)
>       - wachtwoord (varchar:60)
>       - team (int:3)
>       - contributie (int:1)
> 4. [ ] Zet gegevens in deze tabel.

> ##### Teams
> 
> 1. [ ] Maak nog een tabel: `teams`
> 2. [ ] Maak de volgende _kolommen_ aan: 
>       - id (int:11)
>       - naam (varchar:100)
> 3. [ ] Zet gegevens in deze tabel.

> ##### Pagina's
> 
> 4. [ ] Maak een database bestand: db.conn.php
> 5. [ ] Maak een pagina om alle leden te kunnen tonen
> 6. [ ] Maak een pagina om teams te kunnen bekijken
> 7. [ ] Maak een pagina om de gegevens van een enkele gebruiker te kunnen tonen
> 8. [ ] Maak een pagina om de gegevens van een enkel team te kunnen tonen


## Eindresultaat

Het eindresultaat is een volledig werkende webapplicatie die de overzichten van `teams` en van `gebruikers` kan tonen. Daarnaast ook de _profiel_ pagina's van individuele entiteiten.

## Bronnen

Een lijstje van links naar externe bronnen

> Bijvoorbeeld:  
> [W3 Schools - PHP Functions](https://www.w3schools.com/php/php_functions.asp)  
> [Jaap van der Veen - PHP Basiscursus Les3: Functies](https://phpbasis.jaapvdveen.nl/basiscursus-php/les-3-inleiding-functies/)
