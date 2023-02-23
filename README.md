# CSS to the Rescue @cmda-minor-web 2022 - 2023

Voor het vak CSS to the Rescue ga ik een modulair bedieningspaneel maken met CSS. Ik wil hierbij de focus leggen op het animeren, en die animaties zo realistich mogelijk maken. 

### Inspiratie
<img src="/readmeimgs/inspiratie.png" width=500px>

Dit is een codepen die Sanne liet zien, ik was erg onder de indruk dat het allemaal mogelijk is met CSS. Ik wil kijken of ik dit ook kan, maar dan met meerdere controls.

## Week 1 voortang
In de eerste week heb ik mijn opdracht keuze, en mijn focus doorgegeven tijdens het voortgangs gesprek. Voor de volgende week wil ik de basis van de HTML hebben staan en een idee hebben wat voor functionaliteiten ik mee wil beginnen. Ik wil hier gelijk mee starten en proberen een basis CSS toe te voegen.

## Week 2
In week 2 ben ik begonnen met de setup van de HTML. Eerst heb ik een kleine tekening gemaakt zodat ik een kleine start heb. Daarna vond ik het lastig om aan de CSS te beginnen. Ik wist niet zo goed waar ik nou moest starten.

<img src="/readmeimgs/design.jpg" width=500px>

Ik ben uiteindelijk eerst gestart met het maken van de functionaliteiten van het bedieningspaneel. Ik heb doormiddel van checkboxes en de :has CSS selector voor elkaar gekregen dat ik een lamp aan en uit kan laten gaan. Daarna heb ik proberen een slider te stylen (Input type range). Waar ik achter ben gekomen is dat je (orient="vertical") kan toevoegen in de HTML om hem verticaal te krijgen, maar dit werkt alleen in firefox, en de :has selector werkt daar weer niet in. Om het in alle browsers te laten werken heb je een transform rotate nodig.

<img src="/readmeimgs/voortgang1.png" width=500px>

Voor het volgende feedback gesprek wil ik alle functionaliteiten af hebben en begonnen zijn met de styling van het paneel. 

## Week 3
In week 3 ben ik verder gegaan aan de functionaliteiten van het paneel. Het is gelukt om een hendel toe te voegen om de lamp omhoog en omlaag te laten gaan, maar ook heb ik een grote rode knop en een slider toegevoegd. Waar ik vast was gelopen was het maken van de hendel. Het animeren lukte mij niet echt. Hoe ik dit heb opgelost is twee animaties toevoegen, en eentje reverse laten afspelen.

<img src="/readmeimgs/voortgang2.png" width=500px>

De hendel deed lastig met positioneren, maar het is uiteidenlijk toch gelukt om het werkend te krijgen. Ook heb ik er wat meer detail aan toegevoegd, maar het is nog lang niet iets waar ik tevreden mee ben.

De slider is ook iets waar ik moeite mee had. Voor de slider mocht er javascript gebruikt worden, maar met een scriptje die al geschreven was. Dit dat op de head van de HTML, en wist niet zo goed hoe ik dit eruit moest halen. Uiteindelijk heb ik het kunnen oplossen door gebruik te maken van css selectoren.

```css
    head[data--x="10"] + body header > section div
```


<img src="/readmeimgs/voortgang3.png" width=500px>
 
Verder heb ik de kleur knopjes even weg gelaten om te focussen op andere dingen. De slider, knop en hendel werken nu allemaal.

Voor week 4 is het de bedoeling om alles af te krijgen. Het enige wat nu nog te doen staat is de animaties wat vloeiender te maken, en wat meer detail toevoegen aan ieder opbject



