1. De beste manier om deze app te maken is met behulp van een scherm dat alles controleert. Open Screen1.

2. Dit scherm heeft ook een **Bestand** nodig, voeg er één toe.

3. Ga naar de Blokken editor. Je gaat je eerste procedure maken! Een procedure is een stukje code dat je kunt gebruiken met het "roep aan" blok. Meestal zullen programmeurs deze blokken gebruiken zodat ze niet steeds dezelfde code moeten maken. Deze blokken gaan we gebruiken:  
   ![](/nl/assets/AI14.jpg)

4. Klik op **Procedures** aan de linkerkant en sleep het `tot [procedure]` blok in je scherm. Je gaat minigames openen met deze procedure, dus om je te helpen onthouden wat deze procedure doet, noem je het "openMinigame".

5. Aangezien je een scherm opent, sleep je het **Controle** blok `open een ander scherm schermNaam` naar het **Procedure** blok.

6. Deze procedure gaat voor al jouw minigames werken. Sleep het blok `initializeer globaal [naam] `blok uit de **Variabelen** naar het scherm. Verander "naam" naar "aantalMinigames" \(zo weet je waar de variabele voor is\). Sleep het `[0]` blok erin en verander de 0 in 2 \(het aantal minigames dat je tot nu toe hebt\) en dan is deze variabele klaar.  
   Het moet er zo uit zien:  
   ![](/nl/assets/AI15.jpg)

7. De laatste stap betreft het kiezen van een scherm! Weet je de namen van je eerste twee minigames nog? Minigame1 en Minigame2. Hierdoor kun je willekeurig een scherm kiezen. Door willekeur toe te voegen voelt je app elke keer anders aan.

8. Om willekeurig een minigame te kiezen heb je vier blokken nodig: een `samenvoegen` blok uit **Tekst** \(dit voegt twee teksten samen\), `willekeurig getal tussen [1] en [100]` vanuit **Wiskunde**, een `krijg [ ]` blok uit **Variabelen** en een **Tekst**blok met de tekst "Minigame". Zet ze allemaal als volgt in elkaar:![](/nl/assets/AI16.jpg)



