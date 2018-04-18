1. Jij hebt alle controle over de werking van je app! Nu is het heel makkelijk om je eigen minigames toe te voegen. We geven je nog een voorbeeld en daarna ga je zelf aan de slag.

2. Maak een "Minigame3" scherm.

3. Dit spel laat de speler raden naar een optelsom. Dus je hebt twee labels, één tekstblok en een knop nodig in de **Ontwerper**. Zo ziet die van ons eruit:  
   ![](/nl/assets/AI25.jpg)

4. Ga naar Blokken. Gebruik een **voor elk lus** om het programmeren van het spel makkelijker te maken. Elke 'voor elk' lus herhaalt dezelfde code tot het stopgezet wordt. Dit is handig voor luie programmeurs!

5. Gebruik een `wanneer [Minigame3].Initialiseer `blok en zet daar een `Initialiseer lokaal [naam] tot` blok in. Verander "naam" in "getalTekst" en voeg een leeg `" "` blok toe.

6. Voeg nu een `voor elk [getal] van` blok toe \(in **Controle**\). Dit blok heeft drie delen. Het eerste is het getal waarmee begonnen moet worden; het tweede hoe lang de lus blijft tellen tot het stopt; en de laatste is hoeveel de lus elke keer optelt \(dit is wat de speler moet raden\). Zet het eerste blok op 0,  het tweede op 10, het laatste op 2:  
   ![](/nl/assets/AI26.jpg)

7. Binnen de lus kun je nu iets gaafs doen! Gebruik het `zet [getalTekst] tot` blok. Je gaat het zetten op de vorige getalTekst en een spatie \(" "\) + het getal \(dit komt uit de voor lus\).

8. Nu moet je tekst van het label naar `krijg [getalTekst] `zetten en moet alles er zo uit zien:  
   ![](/nl/assets/AI27.jpg)

9. Deze stap heb je al eerder gedaan, dus kijk of je begrijpt waarom deze blokken in de code moeten staan:  
   ![](/nl/assets/AI28.jpg)

10. Ga terug naar Screen1 en zorg dat het `Initializeer globaal [aantalMinigames] tot` blok nu op 3 staat \(je hebt nu immers drie spellen!\)

11. Zie je hoe makkelijk het was om een spel toe te voegen? Probeer deze ideeën eens uit:

    * Bedenk zelf een spel \(dat is altijd leuker\).

    * Verander de lijst minigame. Laat het spel willekeurig een object uit de lijst kiezen, zeg de speler erop te klikken en kijk na of de speler de juiste keuze maakte.

    * Probeer andere **Media** opties uit. Je kunt de speler vragen een foto van zichzelf te maken met de camerablokken.

    * Kijk of het de speler lukt om in één seconde vijf keer op een knop te drukken.

    * Probeer van alles uit, gebruik je fantasie en probeer alle blokken!



