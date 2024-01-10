---
title: 'Kwantitatieve gegevensverwerking met Jamovi'
subtitle: 'Onderzoeksskills 2'
date: "10/01/2024"
date-format: "YYYY"
author: "dr. Willem De Keyzer"
toc-title: "Inhoud"
abstract: |
    Aan het einde van deze modele zul je de volgende tools en functies van Jamovi kennen:

    - Navigeren door en gebruikmaken van de Jamovi-omgeving 
    - Variabelen en cases verkennen en maken 
    - Beschrijvende gegevensverwerking 
    - Eenvoudige grafieken en boxplots 
    - Parametrisch testen

    ::: Questions
    Doorheen de module zijn er **leercontroles** (genummerd Q1, Q2, enz.) die je vragen stellen over wat er zojuist is behandeld. Deze vragen worden niet gesteld ter beoordeling, maar om je te helpen Jamovi volledig te leren gebruiken. De antwoorden op alle vragen staan aan het einde van deze module zodat je kunt controleren of je het goed hebt gedaan en je kunt op de vraagnummers klikken om naar dat antwoord te gaan.
    :::
---

\wordtoc

# Vertrouwd raken met Jamovi

In dit gedeelte zullen we vooral wennen aan het gebruik van Jamovi en het instellen van onze gegevens.

## Jamovi op je eigen computer installeren

Omdat Jamovi een gratis en open-source applicatie is, kan je deze eenvoudig op je eigen computer installeren. Download het Jamovi-installatieprogramma voor jouw systeem van:

[https://www.jamovi.org/download.html](https://www.jamovi.org/download.html)

Als je de optie krijgt, kies dan de versie '**Solid**'. Zodra het installatieprogramma is gedownload, dubbelklik je erop om Jamovi op je computer te installeren. Voor een volledige handleiding en instructies voor het installeren van Jamovi, zie sectie 1 van de **Jamovi-gebruikershandleiding** hier:

[https://www.jamovi.org/user-manual.html](https://www.jamovi.org/user-manual.html)

Jamovi is een gewone applicatie-installatie voor Windows en Mac, maar Jamovi is ook beschikbaar voor Linux en Chromebooks met enkele extra stappen (zie de bovenstaande gebruikershandleiding voor meer informatie). Als je Jamovi om de een of andere reden niet op je computer kunt installeren, kun je hier een online versie van Jamovi gebruiken:

[https://cloud.jamovi.org/](https://cloud.jamovi.org/)

::: Aside

Houd er rekening mee dat de online versie van Jamovi slechts een demoversie is en niet altijd beschikbaar is. Het wordt **sterk aanbevolen** om Jamovi op je eigen computer te installeren als dat mogelijk is.

:::

## Hulp met Jamovi

Jamovi heeft veel online hulpbronnen om je te helpen bij het gebruik! Naast de gebruikershandleiding waarnaar hierboven wordt verwezen, kan je hier een aantal nuttige gidsen vinden op de pagina met hulpmiddelen van de Jamovi-gemeenschap:

[https://www.jamovi.org/community.html](https://www.jamovi.org/community.html)

Er is met name een YouTube-afspeellijst met nuttige Jamovi-videogidsen ([klik hier](https://bit.ly/jamovi-youtube)) en een volledig handboek over statistiek met Jamovi ([klik hier](https://www.learnstatswithjamovi.com/)) gelinkt aan de pagina met hulpmiddelen van de community die handig kunnen zijn als je hulp nodig hebt buiten een tutorial om, of als je nog meer details wilt weten over statistiek met Jamovi.

## Download de gegevensbestanden

Download **alle** Jamovi-gegevensbestanden van [GitHub](https://github.com/wdkeyzer/jamovi-worksheets/tree/master/00-Data-Files) en sla ze ergens op waar je er gemakkelijk bij kunt.

Jamovi gebruikt de '.omv' bestandsextensie, wat een aangepast bestandsformaat is. In tegenstelling tot andere bestandsformaten kun je deze niet dubbelklikken als snelkoppeling om ze in Jamovi te openen - maak je geen zorgen, je moet gewoon eerst Jamovi openen en ze dan vanuit Jamovi openen.

## Eerste kennismaking met Jamovi

Open na de installatie de Jamovi-toepassing. Je zou een lege Jamovi-werkruimte moeten zien:

![](_imgs/01-01.png)

De werkruimte in Jamovi is verdeeld in een aantal secties.

- Het grote rasterachtige gebied aan de linkerkant (dat eruit ziet als Excel) is het **Spreadsheet**. Hier komen je gegevens te staan!
- Het lege gebied aan de rechterkant is de **Results Viewer**. Dit is een blanco vel papier waarop Jamovi de resultaten afdrukt van alle tests die je uitvoert. Je zult binnenkort zien hoe dit werkt.
- Bovenaan staat het **Menu**. Dit heeft een paar opties - **Data**, **Analyses** en **Edit**. We zullen vooral Data en Analyses gebruiken. Als je op een van deze opties klikt, verandert het **lint** direct eronder om te laten zien wat je met elke optie kunt doen - in de schermafbeelding hierboven hebben we **Analyses** geselecteerd, dus het lint toont ons alle verschillende Analysetests die we kunnen uitvoeren.

Het menu heeft ook drie gestapelde witte lijnen in de linkerhoek - dit opent het **File** menu. Klik daar nu op, klik dan op **Open**, vervolgens op **Browse** en navigeer naar de plaats waar je alle gegevensbestanden van hebt opgeslagen:

![](_imgs/01-02.png)

Open het bestand **Body Composition.omv**.

Je zou nu gegevens moeten zien in de Spreadsheet-weergave. Als je meer gegevens wilt zien, kan je de grootte van de Spreadsheet en Results Viewer aanpassen door de dikke grijze lijn in het midden van het scherm aan te klikken en te verslepen.

![](_imgs/01-03.png)

## Cases en variabelen

In Jamovi staat elke **kolom** voor een **variabele**, net als in Excel, en elke **rij** voor een **case** (eenheid). Vergeet niet om persoonlijke gegevens minstens te pseudonimiseren door een anoniem nummer te gebruiken. In dit bestand wordt deze variabele 'PartID' genoemd.

::: Questions
[Q1]{}. Hoeveel kolommen met gegevens zijn er?

[Q2]{}. Hoeveel rijen gegevens zijn er?

[Q3]{}. Waarom een deelnemers-ID als er een recordnummer is?

[Q4]{}. Waarom hebben we hoe dan ook een deelnemers-ID nodig? Waarom gebruiken we niet gewoon de naam van de deelnemer?
:::

Bekijk de kolom PartID - merk op dat sommige ID's ontbreken, zodat het rijnummer niet altijd overeenkomt met het nummer Participant ID  (PartID).

Voeg nog een eenheid toe aan de gegevens, typ de volgende nummers onderaan het blad. Je kunt rechtstreeks in elke cel typen (vergelijkbaar met Excel).

- PartID: 53
- Age: 21
- Gender: 2
- Course: [laat leeg]
- Weight: 41.0
- Height: 160.0
- BIA1: 18.8
- BIA2: 18.8
- FitPercept: [laat leeg]

### Variabelen instellen

Tot nu toe gedraagt het gegevensblad zich ongeveer zoals Excel wat betreft wat we kunnen invoeren. Maar in tegenstelling tot Excel kunnen we in Jamovi meer informatie invoeren over wat er in elk van onze variabelen (de kolommen in het gegevensblad) staat. Dit staat bekend als **metadata**. Om deze te bewerken, klik je op **Data** en vervolgens op **Setup** (het pictogram dat eruitziet als een tandwiel bovenop een mini gegevensblad). Er wordt een extra menu geopend bovenaan het Jamovi-scherm:

![](_imgs/01-04.png)

Bovenaan zie je in grote tekst de naam van de variabele die we aan het bewerken zijn. Dit is de variabele **Label**. Klik op een cel in een andere kolom om naar die variabele te gaan - zie hoe de tekst bovenaan het menu voor het instellen van variabelen verandert.

Direct onder het grote Label-gebied staat nog een tekstvak - dit is het **Beschrijving**-gebied, waar je wat extra tekst kunt toevoegen om duidelijker te maken wat er in onze variabele staat. Klik op de kolom PartID en zie hoe er nu 'Participant ID' staat - dit is de volledige naam van de variabele, in plaats van het kortere label 'PartID'.

::: Aside

Waarom gebruiken we aparte labels en beschrijvingen? Wanneer je met een variabele werkt, kan het soms vervelend zijn om de volledige naam steeds opnieuw in te typen - 'PartID' is veel sneller in te typen dan 'Deelnemer-ID'. Maar als we onze resultaten willen zien, willen we de volledige beschrijving van de variabele, zodat het makkelijker en duidelijker is om te zien waar onze resultaten naar verwijzen.

:::

Wijzig nu een paar variabele eigenschappen:


- Je ziet dat de meeste van onze variabelen een Naam en Beschrijving hebben, maar er ontbreken er twee. Voer voor de kolom **Age** de beschrijving 'Age (years)' in en voer voor de kolom **Gender** de beschrijving 'Gender' in.

### Variabele gegevenstypen

Onder de beschrijving staan nog enkele opties. Klik op het dropdownmenu naast **Measure type**:

![](_imgs/01-05.png)

::: Questions
[Q5]{}. Hoeveel datatypes zijn er beschikbaar in Jamovi?
:::

Jamovi heeft drie hoofdtypen gegevens:

- Nominaal
- Ordinaal
- Continu

Nominaal en Ordinaal zijn precies hetzelfde als de meetniveaus die je elders vindt. Continu' is gewoon de combinatie van Interval en Ratio - Jamovi rekent achter de schermen uit of de gegevens die je invoert Interval of Ratio zijn, op basis van de getallen in de gegevens.

Jamovi heeft ook een extra gegevenstype, genaamd 'ID'. Dit wordt gewoon gebruikt door Jamovi om een Deelnemer ID kolom te identificeren - het is precies hetzelfde als een Nominale kolom, maar laat Jamovi weten dat het zich geen zorgen hoeft te maken over het labelen van niveaus en dat het gewoon moet gebruiken wat er in de cellen wordt getypt. Maak je niet te veel zorgen over het verschil - weet alleen dat je je PartID kolom alleen op 'ID' hoeft in te stellen.

::: Questions
[Q6]{}. Waarom zou PartID van het type ID of Nominal zijn, ook al lijkt het een geordende lijst van getallen te zijn?
:::

Klik onder de opties voor het meetniveau op het vervolgkeuzemenu voor **Data type**:

![](_imgs/01-06.png)

Gegevenstypen vertellen Jamovi wat voor soort gegevens we gaan invoeren in de cellen van het gegevensblad. Deze zouden vrij duidelijk moeten zijn:

- Integer: gehele getallen zonder decimaalteken (1, 2, 3, ...)
- Decimal: getallen met een decimaalteken (1.5, 2.3, 3.0, 4.6, ...)
- Text: woorden (Ja, Nee, John Smith, voetbal, ...)

We zullen het gedeelte 'Missing values' voorlopig negeren.

### Codering value labels

Tot slot staat rechtsonder in de variabelenviewer de instelling **Levels**. Hier kunnen we, als we categorische gegevens gebruiken (d.w.z. nominale of ordinale gegevenstypen), de labels instellen die moeten verschijnen voor elk niveau van die categorie.

Klik bijvoorbeeld op de kolom **Gender** terwijl het venster Variable setup geopend staat. Merk op hoe de gegevens worden ingevoerd als de getallen 1 en 2, in plaats van als tekst. Verander het **Measure type** in 'Nominal' en je zou de getallen 1 en 2 moeten zien verschijnen in het vak Levels.

![](_imgs/01-07.png)

Klik op het getal 1 in het vak Levels om het label voor deze waarde in te voeren. Verander dit van een '1' in het woord 'Male'. Klik op het nummer 2 en verander het in 'Female'.


![](_imgs/01-08.png)

Merk op hoe de nummers 1 en 2 naar rechtsonder de tekst die je typt verschuiven, zodat je nog steeds kunt zien welk label naar welk nummer verwijst. Klik ergens buiten het labelsvak om deze labels op te slaan.

Merk nu op dat de cellen in de kolom Gender in het gegevensblad veranderen van '1' en '2' in 'Male' en 'Female'. De onderliggende gegevens zijn nog steeds hetzelfde - we hebben ze alleen gelabeld.

::: Aside

Waarom getallen en labels gebruiken voor nominale gegevens? Net als bij de namen en labels van onze variabelen, maakt het het makkelijker om met de gegevens te werken en toch onze resultaten duidelijk af te lezen. Als we bijvoorbeeld alleen de mannelijke deelnemers aan dit onderzoek willen selecteren, kunnen we filteren op 'Gender = 1', maar onze resultaten zouden nog steeds het volledige label 'Male' bevatten.

:::

Ga nu door en controleer of alle variabelen in ons gegevensblad correct zijn ingesteld. Zorg ervoor dat de variabelen overeenkomen met de volgende:

-   Age: Age (years), Continuous, Integer
-   Gender: Gender, Nominal, Integer, with 2 levels
-   Course: Course Name, Nominal, Integer, with 4 levels
-   Weight: Weight (kg), Continuous, Decimal
-   Height: Height (cm), Continuous, Decimal
-   BIA1: BIA Machine 1 Body Fat (%), Continuous, Decimal
-   BIA2: BIA Machine 2 Body Fat (%), Continuous, Decimal
-   FitPercept: Fitness Perception, Nominal, Integer, with 5 levels

Als je al deze variabelen hebt ingesteld, klik je op het cirkelpictogram met een pijl omhoog rechtsboven in het menu voor het instellen van variabelen om het menu te verbergen en terug te keren naar de hoofdweergave.

Zorg ervoor dat je je gegevens regelmatig opslaat - klik op de drie witte lijnen linksboven om het menu File weer te openen en klik vervolgens op **Save**.

::: Tip

Gebruik Ctrl + S in Windows of Cmd + S op Mac als sneltoets om je werk op te slaan. Zorg ervoor dat je regelmatig opslaat om te voorkomen dat je iets kwijtraakt! Al je gegevens, tests en resultaten worden opgeslagen in hetzelfde .omv-bestand, zodat je het later weer kunt openen en verder kunt gaan waar je gebleven was.

:::

### Een nieuwe variabele berekenen

We ontbreken nog een BMI-variabele, dus gaan we er een maken. Je zou alle gegevens in Excel kunnen maken en ze dan kopiëren en plakken in Jamovi, maar Jamovi heeft een functie **Compute variable** die de berekening voor ons kan uitvoeren.

Klik op de kolom **FitPercept**, klik vervolgens op **Data** en vervolgens op **Compute** (het pictogram dat eruitziet als een rekenmachine). Dit voegt een nieuwe kolom toe na de kolom waar onze cursor staat (daarom hebben we eerst op FitPercept geklikt) en opent het menu **Computed  variabele** bovenaan, vergelijkbaar met het menu voor het instellen van variabelen:


![](_imgs/01-09.png)

Jamovi geeft onze variabele automatisch een letter van het alfabet als naam - 'J' in dit geval. Verander de nieuwe variabelenaam in **BMI** en voer vervolgens **Body Mass Index** in als beschrijving.

Onder de naam en beschrijving staat het vak **formule box**. Hier voeren we een formule in om Jamovi te vertellen wat hij voor ons moet berekenen - heel vergelijkbaar met wanneer we functies in Excel typen, maar in plaats van ze in één cel te typen en de formule in alle andere cellen te kopiëren en plakken, voeren we in Jamovi gewoon de functie bovenaan in en wordt deze automatisch voor de hele kolom voor ons ingevuld.

We kunnen direct in het formulevak typen of Jamovi sommige delen voor ons laten invullen. Klik op de **fx** knop om alle opties te zien die we in het formulevak kunnen invoeren:


![](_imgs/01-10.png)

Jamovi vertelt ons wat elke functie doet als we er één keer op klikken - zie hier dat ik op de MEAN-functie heb geklikt, en Jamovi geeft er een korte beschrijving onder. Naast de functies staan onze variabelen. Dubbelklik op deze variabelen om ze in te voegen in het functievak.

Typ of kopieer en plak nu het volgende in het functievak:

```
Weight / ((Height/100) * (Height / 100))
```

![](_imgs/01-11.png)

Druk op enter en je zou moeten zien dat de BMI kolom automatisch wordt ingevuld met onze BMI waarden. Merk op dat alle cases (rijen) die geen gewichts- of lengtegegevens hebben, ook leeg blijven in de nieuwe BMI-kolom.

**Even samenvatten:** we hebben gekeken naar het gegevensblad dat onze gegevens (cellen) bevat gerangschikt als Variabelen (kolommen) en Cases (rijen). We hebben in het menu Variable Setup gekeken naar de metadata-informatie over onze variabelen en de waarden die ze bevatten. Dit zijn de twee hoofdcomponenten van wat we gegevens zouden noemen.

De variabelen en de gegevens worden allemaal opgeslagen in één Jamovi-gegevensbestand (.omv). Zorg ervoor dat je je gegevensbestand opslaat wanneer je wijzigingen hebt aangebracht in zowel de variabelen als de cases. We gaan nu verder met het onderzoeken van enkele van onze gegevens.

::: Aside

Gebruik het **File** menu van eerder om je werk op te slaan - klik op de drie gestapelde witte lijnen in de hoek en kies **Save** of **Save as**. U kunt ook de sneltoetsen **Ctrl + S** (Windows) of **Cmd + S** (Mac) gebruiken om op te slaan.

:::

\newpage

# Beschrijvingen, plots en parametrische tests

Nu we onze gegevens hebben ingesteld in Jamovi, kunnen we ze gaan onderzoeken met wat beschrijvende grafieken, wat basisplots en wat parametrische tests.

## Beschrijvende gegevens

Dit is informatie over je gegevens, bijvoorbeeld het totale aantal records, het minimum, maximum, bereik, standaardafwijking, enz. Jamovi kan deze informatie veel sneller leveren dan dat we het elke keer zelf moeten uitrekenen. Hier gaan we een aantal verkennende analyses gebruiken om onze gegevens te beschrijven.

Klik in het menu **Analyses** op het pictogram **Exploration** (dat eruitziet als een staafdiagram) en klik vervolgens op **Descriptives** in het vervolgkeuzemenu dat verschijnt. Er wordt nu een nieuw middengebied geopend tussen ons werkblad en de resultatenviewer:

![](_imgs/01-12.png)

Merk op dat er ook iets is verschenen op onze resultatenviewer! Dit is hoe Jamovi werkt - als je een analyse uitvoert, worden de resultaten afgedrukt op de viewer aan de rechterkant. De "descriptives" drukt standaard een tabel met informatie af, maar op dit moment hebben we Jamovi nog niet precies verteld waarvan we descriptives willen, dus de tabel is leeg.

Klik op de variabele **Weight** in het linkervak en klik op de pijl om deze te verplaatsen naar het vak **Variables** aan de rechterkant. Klik vervolgens op de variabele **Gender** en verplaats deze met de pijl naar het vak **Split By**:
![](_imgs/01-13.png)

Dit is een eenvoudige manier om alle gewichten van onze deelnemers (afhankelijke lijst) uitgesplitst naar geslacht (factorlijst) te bekijken.

Merk op dat onze resultatentabel aan de rechterkant nu automatisch is bijgewerkt om de beschrijvingen weer te geven waar we om hebben gevraagd! Je zou het gemiddelde, de mediaan, de standaardafwijking, het minimum en het maximum moeten kunnen zien voor zowel de mannelijke als de vrouwelijke groep. Deze vereisen allemaal aparte vergelijkingen in Excel, dus je kunt zien dat Jamovi *veel sneller* is om gegevens samen te vatten.

::: Questions
[Q7]{}. Wie is er gemiddeld zwaarder in deze dataset, mannen of vrouwen?

[Q8]{}. Hoeveel mannen en vrouwen zijn er? En hoe groot is onze totale steekproefomvang?
:::

Laten we nog wat meer van onze gegevens bekijken. Eerder zagen we det we twee kolommen hadden, BIA1 en BIA2, waar we het lichaamsvetpercentage hebben gemeten met twee 'identieke' apparaten. Hier kunnen we deze twee velden kort bekijken om eventuele verschillen te vergelijken.

Klik op **Weight** in het variabelengebied en zie dat het pijlpictogram naar links wijst - klik hierop om het terug te zetten in onze variabelenlijst. Doe hetzelfde voor **Gender**. De tabel in onze Results viewer zou nu weer leeg moeten zijn.

Selecteer nu **BIA1** en **BIA2** en verplaats ze naar het vak Variabelen. Dit toont dezelfde informatie als eerder, maar nu willen we een beetje extra. Klik op het vervolgkeuzemenu **Statistics** onder onze variabelenkiezer om alle verschillende statistieken te zien die we Jamovi kunnen laten weergeven. Klik op **Range** om het toe te voegen aan onze tabel in de resultatenviewer:

![](_imgs/01-14.png)

Klik gerust rond alle andere statistische opties waarin je geïnteresseerd zou kunnen zijn - je kunt er zoveel toevoegen en verwijderen als je wilt op elk moment in Jamovi, en de resultatenviewer zal automatisch worden bijgewerkt om te laten zien wat je hebt gewijzigd.

::: Questions
[Q9]{}. Zou je op basis van de beschrijvende gegevens voor de twee machines zeggen dat de machines 'dezelfde' resultaten laten zien?
:::

### Frequentietabellen

Laten we ook eens kijken hoeveel studenten er in elk van de vier aangeboden cursussen zitten. Verplaats BIA1 en BIA2 uit de geselecteerde variabelen en verplaats **Course** naar het selectievakje voor variabelen.

Klik op het selectievakje **Frequency tables** onder onze variabelen selectie om een frequentietabel toe te voegen aan onze resultatenviewer (dit werkt alleen voor nominale of ordinale gegevenstypen). Als je de resultatenviewer wat netter wilt maken, verwijder dan het vinkje bij alle andere Statistics-opties, maar laat de opties **N** en **Missing** staan:

![](_imgs/01-15.png)

Hier zie je de frequentie als een telling, als een algemeen percentage en als een cumulatief percentage. De bovenste tabel vertelt ons ook over het totale aantal waarden en hoeveel waarden er ontbreken - dat wil zeggen, alle gevallen die we hebben zonder inschrijving in een cursus.


::: Questions
[Q10]{}. Hoeveel studenten hebben daadwerkelijk een cursusnaam opgegeven?

[Q11]{}. Welke cursus heeft het grootste percentage studenten?

[Q12]{}. Welk percentage studenten volgt Sport and Dance Therapy?
:::

Merk op dat onze tellingen in de frequentietabel optellen tot het aantal geldige waarden in onze gegevens. Je moet altijd controleren op ontbrekende waarden in je gegevens - in dit geval moet je misschien teruggaan en die ontbrekende cursus vinden, of anders deze case uitsluiten van verdere analyses als een cursusnaam vereist is.

## Basisgrafieken

We zullen twee grafieken bekijken:

- Histogram
- Boxplot

### Histogram

We blijven onze gegevensreeks Body Composition.omv gebruiken. Nog steeds in het **Descriptive** menu, wis je alle variabelen uit onze variabelenselectie en vink je de optie Frequentietabel uit. Verplaats **Weight** naar de variabelen selectie en schakel de Default descriptive statistics weer in - vink de vakjes aan voor N, Missing, Mean, Median, Std. Deviation, Minimum en Maximum.

Klik vervolgens weer op de menubalk Statistics om deze weg te klappen en klik op de menubalk **Plots**. Klik op **Histogram** om een eenvoudig histogram te genereren in onze resultatenviewer.

![](_imgs/01-16.png)

Dit is een histogram voor onze hele gegevensverzameling, maar we kunnen dit opsplitsen naar **Gender**, precies zoals we hebben gedaan voor de Beschrijvende gegevens. Verplaats Gender in het vak Splitsen op en kijk wat er gebeurt met ons histogram:

![](_imgs/01-17.png)

Je kunt je gegevens splitsen met elke nominale of ordinale variabele - probeer andere variabelen in en uit het vak Split By te verplaatsen om te zien hoe het histogram verandert.


::: Questions
[Q13]{}. Gebaseerd op de histogrammen, welk Geslacht heeft een grotere variabiliteit in gewicht? Waarom?
:::

### Boxplots

Boxplots kunnen ook nuttig zijn om je gegevens visueel te inspecteren, vooral als je op zoek bent naar uitschieters. We zullen een boxplot gebruiken om te controleren op uitschieters in onze lengtegegevens. Wis de selectievakjes, verplaats **Height** naar de selectie van variabelen en splits opnieuw op **Gender**. Klik vervolgens op het selectievakje **Boxplot** om een boxplot weer te geven in de resultatenviewer:

![](_imgs/01-18.png)

Denk eraan in een boxplot (box and whisker plot):

- Bovenste whisker (snorhaar) = 1,5 x interkwartielafstand
- Bovenste vak = 3e kwartiel
- Lijn in het midden = mediaan
- Onderste vak = 1e kwartiel
- Onderste whisker = 1,5 x interkwartielafstand

Uitschieters worden weergegeven met cirkels buiten de whiskers van de boxplot. Er zijn geen uitschieters in onze lengtegegevens.

::: Questions
[Q14]{}. Wat is op de boxplot bij benadering de waarde voor de lengte van de man en de lengte van de vrouw?
:::

Klik nu gerust op andere Plot- of Statistiekopties die je interessant vindt en probeer verschillende variabelen en manieren om de gegevens op te splitsen. Vergeet niet dat als je iets wilt verwijderen uit de resultatenviewer, je gewoon het vinkje weghaalt.

## Parametrisch testen en voorwaarden

Voordat we kunnen beslissen welke test we gaan gebruiken, moeten we kijken naar de 'kwaliteit' van onze gegevens.

Er zijn 4 aannames waar we naar moeten kijken:

- Meetniveau van de variabele
- Onafhankelijkheid van gegevens (vaak willekeurige toewijzing van gegevens genoemd)
- Normale verdeling
- Homogeniteit in variantie

:::Warning
Onthoud dat als je meerdere variabelen vergelijkt, je elke variabele (of gesegmenteerde variabele) moet toetsen aan je aannames.
:::

### Testen op normaalverdeling

Hoewel we eenvoudigweg naar een histogram kunnen kijken om visueel te controleren of er sprake is van een normaalverdeling, zijn er een ook aantal statistische tests die we kunnen uitvoeren. De belangrijkste statistische test voor normaliteit in Jamovi is de **Shapiro-Wilk** (SW) test.

Laten we de verdeling van de lengtegegevens van mannen en vrouwen onderzoeken. Om de twee sets onafhankelijke gegevens te vergelijken, moeten we ervoor zorgen dat zowel de mannelijke als de vrouwelijke gegevens niet significant afwijken van een normale verdeling. *(Opmerking: het testen van gegevens met herhaalde maten vereist een iets andere test, maar hier zullen we de normaalverdeling voor onafhankelijke steekproeven onderzoeken en later kijken naar afhankelijke gegevens)*

Nog steeds in het menu Descriptives verplaatst je **Height** naar de selectie van variabelen en splits je de gegevens op **Gender**. Klik vervolgens in het menu Statistics op het selectievakje **Shapiro-Wilk**:

![](_imgs/01-19.png)

Hierdoor worden rijen voor Shapiro-Wilk *W* en Shapiro-Wilk *p* waarden toegevoegd aan onze tabel met beschrijvingen in de resultatenviewer.

Hier testen we of de verdeling van de lengte (per geslacht) normaal verdeeld is, zodat we later parametrische tests kunnen gebruiken. We willen zien of er een significante afwijking van de normaliteit is, d.w.z. of het resultaat van de *p* waarde kleiner is dan 0,05 voor de lengte voor de mannelijke of vrouwelijke groepen. Beide groepen hebben een *p* \> 0,05. Dit betekent dat er geen significante afwijking is van een normale verdeling, dus aan de normaliteitstest is voldaan.

**Probeer nu:** Voer een normaliteitstest uit voor **Weight** per **Gender** met de gegevensverzameling Body Composition.omv.

::: Questions
[Q15]{}. Welke test zou je uitvoeren?

[Q16]{}. Welke p-waarde voor de normaliteitstest krijg je voor de gewichtsgegevens van de groep vrouwen? Wat betekent deze p-waarde?
:::

Een eenvoudige SW-test is goed om mee te beginnen, maar je moet nog meer controles uitvoeren op je gegevens. De eerste twee die we zullen onderzoeken zijn **Skewness** en **Kurtosis**.

Nog steeds in het Descriptives menu, kies de **Height** variabele opgesplitst in **Gender**. Vink onder Statistieken **Skewness** en **Kurtosis** aan.

![](_imgs/01-20.png)

De eerste manier waarop we deze gegevens kunnen onderzoeken is door te kijken naar de *absolute* waarden voor Skewness en Kurtosis.

- Scheefheid man = 1,028
- Mannelijke kurtosis = 0,959
- Vrouwelijke scheefheid = -0,064
- Vrouwelijke kurtosis = -0,264

::: Questions
[Q17]{}. Beschrijf op basis van de ruwe waarden voor scheefheid en kurtose de vorm van de verdeling van de mannelijke gegevens.
:::

Een vuistregel suggereert dat -0,8 tot +0,8 acceptabel is voor scheefheid en -3 tot +3 acceptabel is voor kurtosis. Merk op dat de scheefheid voor mannen buiten de -0,8 tot 0,8 valt, maar dat alle andere waarden ruim binnen hun bereik liggen. Strikt genomen zouden we kunnen zeggen dat de lengtegegevens van mannen niet normaal verdeeld zijn en een lichte positieve scheefheid vertonen (d.w.z. een opeenstapeling van gegevens aan de linkerkant).

Zet de boxplots voor deze gegevens weer aan. Je ziet de lichte positieve scheefheid voor de mannelijke gegevens met een langere positieve staart:

![](_imgs/01-21.png)

Een andere manier om deze gegevens te onderzoeken is door de lengte scheefheid en kurtosis om te zetten naar een 'gestandaardiseerde' waarde. Dit doen we door de waarde te nemen en te delen door de **standard error** van de waarde. Je kunt de standaardfoutwaarden vinden in de tabel Descriptives, net onder de waarden voor scheefheid en kurtosis.

Deze waarden kunnen nu worden vergeleken met de waarden die we op basis van toeval zouden verwachten, dus een waarde kleiner dan -1,96 of groter dan 1,96 zou betekenen dat deze verdeling significant scheef is of een significante kurtosis vertoont. 


::: Warning

Je kunt deze methode niet gebruiken voor zeer grote steekproeven, omdat de standaardwaarden voor scheefheid en kurtose waarschijnlijk significant zullen zijn, zelfs als de scheefheid en kurtosis slechts weinig afwijken van normaal.

:::

::: Aside

**Normaliteit bij herhaalde metingen:** Met gegevens van onafhankelijke steekproeven, of twee verschillende groepen, moet je de normaliteit van elke afzonderlijke groep controleren. Als je een herhaalde-maatstest hebt, bijvoorbeeld als je groep een test uitvoert onder twee verschillende condities, dan test je niet op de normaliteit van elke groep, maar op de normaliteit van het *verschil* tussen de twee condities.

:::

### Homogeniteit van variantie

Dit is een controle om te zien of de steekproeven die we testen afkomstig zijn van populaties met een vergelijkbare variantie.

Net als bij de normaliteitstest is er een statistische test en een vuistregel. Beginnend met de vuistregel, willen we ervoor zorgen dat de varianties van de twee steekproeven een factor minder dan 3 verschillen.

Stel dat we de lengte van mannen en vrouwen willen vergelijken, dan moeten we de steekproefvariantie van de lengte van mannen en vrouwen vergelijken.

We kunnen deze varianties bekijken in Jamovi - nog steeds met **Height** uitgesplitst naar **Gener** geselecteerd, vink het selectievakje **variance** aan. Hierdoor worden de varianties voor mannelijke en vrouwelijke groepen weergegeven in onze tabel Descriptives in de resultatenviewer.

Om onze vuistregel te testen, neem je de grootste van de twee varianties en deel je deze door de kleinste variantie. In ons geval zou dat zijn:

```
59.4 / 55.649 = 1.07
```

1,07 is ruim binnen onze vuistregel van 3, dus we kunnen homogeniteit van variantie *aannemen*. Maar laten we het ook goed testen. De statistische test die we hiervoor zullen gebruiken is **Levene's Test of Homogeneity**.

Hiervoor moeten we eigenlijk naar een nieuwe menuoptie gaan. Klik op het pijltje naar rechts in de cirkel rechtsboven in het menu Descriptives om het te sluiten. Klik vervolgens, nog steeds in het menu **Analyses**, op het pictogram **T-Tests** en kies **Independent Samples T-Test** in het vervolgkeuzemenu.

Hiermee open je het menu **T-Test**. Je zult zien dat het erg lijkt op het Descriptives-menu - we kiezen bovenaan onze variabelen en hoe we ze willen splitsen (hier **Grouping variable** genoemd) en vinken daaronder de zaken aan die we door Jamovi willen laten zien.

Verplaats **Height** naar onze variabelen selectie en splits weer op **Gender**. Maak je geen zorgen over de andere opties, maar vink de optie **Homogeneity test** aan onder **Assumptions**.

![](_imgs/01-24.png)

Merk op dat dit ons een nieuw gebied geeft in de resultatenviewer, onder het kopje **Independent Samples T-Test**. Maar onze tabel met beschrijvingen wordt er nog steeds boven weergegeven (misschien moet je terug naar boven scrollen). Als je in de resultatenweergave op de tabel met beschrijvingen klikt, wordt het beschrijvende menu weer in het midden geopend en kun je wijzigingen aanbrengen. Dit is de manier waarop je resultaten worden opgeslagen en bewerkt in Jamovi - klik erop in de viewer om het menu voor dat specifieke resultaat te openen. Als je een resultaat helemaal uit de viewer wilt verwijderen, klik je met de rechtermuisknop op de titel en selecteer je 'Remove' in het uitvalmenu.

We zullen ons nu geen zorgen maken over de resultaten van de T-Test - kijk gewoon naar de tabel met de titel **Homogeneity of Variances Test (Levene's)**. Hier kijken we of het testresultaat significant is, net als bij de normaliteitstest. De niet-significante waarde van *p* = 0,901 zegt dat de varianties niet significant van elkaar verschillen en dat we verder kunnen gaan met onze parametrische tests.

**Probeer zelf:** Herhaal de test voor Homogeniteit van Variantie voor Weight per Gender.

::: Questions
[Q18]{}. Wat is de Levene's test en *p* waarde en wat betekent dit?

[Q19]{}. Zou je een parametrische test uitvoeren op deze gegevens? En waarom?

:::

\newpage

# Antwoorden op vragen

::: Questions

[A1]{}. In dit gegevensbestand staan 9 kolommen met gegevens: deelnemer ID, leeftijd, geslacht, cursus, gewicht, lengte, BIA1, BIA2 en FitPercept.

[A2]{}. Er zijn 50 rijen met gegevens, oftewel 50 'cases' (eenheden). Gebruik PartId niet om het aantal records weer te geven.

[A3]{}. Ook al is er een rijnummer, dit identificeert geen specifieke eenheid uit de gegevens, alleen de volgorde van de rijen (of cases) die momenteel worden weergegeven. Met de PartId kan de gebruiker gemakkelijk een bepaalde case identificeren. Als je de gegevens sorteert of filtert, kunnen de rijnummers veranderen, maar PartId blijft consistent.

[A4]{}. Ten eerste zal de PartId uniek zijn, maar het maakt het ook mogelijk om de gegevens te anonimiseren.

[A5]{}. Jamovi heeft vier hoofdtypen gegevens: Nominaal, Ordinaal, Continu en ID. Continu is een combinatie van de gegevenstypen Interval en Ratio. ID is een uniek gegevenstype voor Jamovi, dat alleen wordt gebruikt voor deelnemers-ID-variabelen, dat vergelijkbaar is met een nominaal gegevenstype, maar zonder categorieniveaus of labels.

[A6]{}. Het veld is puur een 'naam' voor elk record, je kunt er niet uit afleiden dat er een volgorde is, of dat het ene voor of na het andere moet komen.

[A7]{}. Vrouwen zijn gemiddeld zwaarder. Gemiddelde massa vrouw = 78.3 kg, gemiddelde massa man = 64.2 kg.

[A8]{}. Er zijn 17 mannen en 31 vrouwen in de steekproef.

[A9]{}. Het is moeilijk definitief te zeggen of de machines 'hetzelfde' laten zien. De beschrijvende informatie zou suggereren dat de waarden 'gemiddeld' hetzelfde zijn, maar afzonderlijke machines binnen de steekproef zouden heel verschillende resultaten kunnen laten zien, bijv. machine 1 geeft 15% en 25% voor twee deelnemers, maar machine 2 geeft 25% en 15% voor dezelfde twee. Gemiddeld' zouden beide machines 20% aangeven. Het feit dat getallen op elkaar 'lijken' betekent niet dat ze statistisch gezien hetzelfde zijn.

[A10]{}. 49 studenten hebben een cursus opgegeven.

[A11]{}. Sport Therapy, met 55,1%.

[A12]{}. 14,3% van de studenten volgt Sport and Dance Therapy.

[A13]{}. Uit de grafiek blijkt dat vrouwen variabeler zijn en zich links en rechts van de mannen in de grafiek uitstrekken. De standaarddeviatie is ook groter voor vrouwen (17,32 kg) vergeleken met mannen (13,84 kg).

[A14]{}. In de boxplot is de mediaan de dikke zwarte lijn in het midden van elk vak. De geschatte waarde voor de mediane lengte bij mannen is 166 cm en bij vrouwen 175 cm.

[A15]{}. Voor een normaliteitstest zou je de Shapiro-Wilk test uitvoeren.

[A16]{}. Voor vrouwen is Shapiro-Wilk *p* = 0,210. Dit is vergelijkbaar met de *p*-waarde voor mannen. Een niet-significante waarde suggereert dat de steekproefverdeling voor het gewicht van vrouwen niet significant verschilt van een normale verdeling, zodat aan een van de aannames voor het uitvoeren van parametrische tests is voldaan.

[A17]{}. De positieve scheefheidswaarde (1,028) suggereert dat de grafiek een iets langere rechterstaart heeft, en de positieve kurtosiswaarde (0,959) suggereert dat de curve iets dunner is dan een normale verdeling (ook wel leptokurtisch genoemd).

[A18]{}. De Levene's test, F = 0,0158, p = 0,901 (gebaseerd op het gemiddelde). Dit betekent dat de varianties niet significant verschillen, dus we kunnen homogeniteit van variantie aannemen.

[A19]{}. Ja, we hebben voldaan aan de vier voorwaarden, 1. Het zijn gegevens van hoog meetniveau, 2. Ze zijn willekeurig toegewezen/selecteerd, 3. Ze zijn normaal verdeeld, en 4. De varianties zijn gelijk.

:::