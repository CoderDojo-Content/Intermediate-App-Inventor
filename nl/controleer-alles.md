1. Je hebt nu alle onderdelen om de app te laten werken! Met deze onderdelen gaan we de app leuk maken.

2. Om controle over de app te houden, hoeft dit scherm alleen maar na te kijken welk scherm net afgesloten is. Dus, sleep het `wanneer [Screen1].AnderSchermGesloten` blok van **Screen1** in je editor.

3. Wanneer een minigame afgesloten wordt, dan geeft dat een waarde. Je kunt deze waarde binnen het `wanneer [Screen1].AnderSchermGesloten` blok zetten.

4. Om de score van de speler bij te houden, kun je het `initializeer globaal [score].tot `blok gebruiken \(in **Variabelen**\). Verander "naam" naar "score" zodat je het makkelijk onthoud. Sleep het `0` blok uit **Wiskunde** naar het `initializeer globaal [score] tot` blok. Zo moet het eruit zien:  
   ![](/nl/assets/AI17.jpg)

5. Sleep het `als dan` blok met het symbool  
   ![](/nl/assets/AI10.jpg)  
   naar je editor. Klik op het radertje en voeg twee `anders als `blokken toe zodat het er zo uit ziet:  
   ![](/nl/assets/AI18.jpg)

6. Het eerste dat nagekeken moet worden is of een minigame of het beginscherm is afgesloten. Gebruik het `[ ] = [ ]` blok uit **Logica**. Kijk of het `resultaat `overeenkomt met de tekst "Beginscherm".

   * NB: dit blok heb je aan het begin toegevoegd en toen uitgeschakeld. Schakel het weer aan zodat het beginscherm sluit met het resultaat "Beginscherm".

7. Voor het `dan` gedeelte wil je een minigame spelen, omdat de enige manier waarop een speler van het beginscherm naar **Screen1** komt is door op de Play knop te drukken. Weet je nog de procedure die je gemaakt hebt? openMinigame? Dat kun je nu gebruiken. In **Procedures** zit nu een `aanroep [openMinigame]` blok, gebruik dat! Je kunt ook het `zet [global score] tot` blok op 0 zetten, zodat de score steeds gereset wordt! Zorg ervoor dat alles klopt:  
   ![](/nl/assets/AI19.jpg)

8. De twee `of als` zullen nakijken of de speler het laatste spel gewonnen of verloren heeft. Onthoud: als een minigame sluit dan resulteert dat in de **Tekst** "gewonnen" of "verloren". Als ze gewonnen hebben, zou de app 1 moeten optellen bij de score van de speler en een andere minigame moeten openen. Je kunt het `[ ] = [ ]`  blok uit **Wiskunde** gebruiken met de scorevariabele om 1 erbij op te tellen.  
   ![](/nl/assets/AI20.jpg)

9. Als ze verloren hebben, slaat het de score op in het bestand en opent het beginscherm. Om de score op te tellen bij het spelersbestand gebruik je het` aanroep [Bestand1].ToevoegenAanBestand `blok \(uit **Bestand1**\). Als de score is opgeslagen opent het beginscherm. Zo zien de blokken er nu uit:  
   ![](/nl/assets/AI21.jpg)

10. Je kunt de app nu uitproberen, maar de score werkt nog niet...dat gaan we op de volgende kaart oplossen!



