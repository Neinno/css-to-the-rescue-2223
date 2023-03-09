# CSS to the Rescue @cmda-minor-web 2022 - 2023

### Link naar live versie
https://neinno.github.io/css-to-the-rescue-2223/index.html

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

## Week 4
Week 4 is de laatste week van CSS to the rescue. In deze week wil ik ervoor zorgen dat alle animaties goed werken, en nog wat extra aandacht geven aan het realistisch maken van mijn paneel. 

Ik ben begonnen met de layout veranderen. Ik heb geprobeerd om met container queries te gaan werken. Dit kreeg ik helaas niet voor elkaar. De code die ik hiervoor wou gebruiken was:

```css
@container (max-width: 450px) {
  form {
    grid-template-columns: 1fr;
  }
}
```

Dit werkte niet voor mij. Uiteindelijk heb ik het niet kunnen oplossen en heb het werkend gekregen met een media query.

Vervolgens ben ik bezig geweest met het meer realistisch maken van de controls van het paneel. Ik heb gekeken naar skeuomorphism en neumorphism om mijn paneel te stylen.

<img src="/readmeimgs/voortgang4.png" width=500px>

Ik heb veel van deze dingen voor elkaar kunnen krijg door gebuik te maken van box shadows en gradients.

Waar ik veel moeite mee had was het oplossen van de animatie van de hendel. Wat het probleem was is dat de stokjes in 3d waren geanimeerd. Daardoor kwamen de stokjes door de hendel heen. Dit heb ik kunnen oplossen door ook op de Z as te animeren.

```css
 transform: translateY(2em) translateX(-50%) translateZ(4em);
```

De hendel word nu ook groter en lijkt ook echt naar je toe te komen. De stokjes komen tijdens de animatie nog steeds een beetje door de hendel heen, maar het is mij niet gelukt dit 100% op te lossen.

## Resultaat:
https://neinno.github.io/css-to-the-rescue-2223/index.html

## Reflectie
Tijdens CSSTTR heb ik veel nieuwe dingen geleerd en geprobeerd. Ik heb in het begin gekozen voor de opdracht bedieningspaneel. Dit heb ik gekozen omdat ik wou ontdekken wat er allemaal mogelijk was met een form. Ik heb geëxperimenteerd met de volgende CSS properties:
- :has selector
- form labels en inputs stylen
- Animeren en keyframes
- Gradients
- Box shadows
- Verschillende manieren om kleuren aan te geven (RGB, Hex, HSL)
- Pseudo-elements en de content property
- @container

Als ik meer tijd had voor de opdracht had ik nog wel wat dingen willen toevoegen. Ik had bijvoorbeeld een animatie willen toevoegen dat de lamp kapot gaat als hij een lange tijd over belast raakt. Ook had ik graag wat meer aandacht willen geven aan de details. Ik had als focus punt het realistisch maken van de controls, maar het is niet helemaal goed gelukt. Toch ben ik redelijk blij met het resultaat. 
