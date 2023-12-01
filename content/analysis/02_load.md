---
Title: Load
Description: Page Loading Speed.
Template: 
---

En Utvärdering av Webbplatsers Laddningstid och Användbarhet
=======================

Denna rapport genomför en utvärdering av tre svenska e-butiker inom skönhetsvård med fokus på deras laddningstid och användbarhet vid internethandel, särskild deras mobilasida.

Urval
-----------------------

De utvalda butikerna är:

- Lyko.se
- Kicks.se
- Bangerhead.se

Dessa tre butiker representerar några av de mest populära inom skönhetssektorn i Sverige. Under de senaste åren har samtliga anpassat sina plattformar för mobilanvändning för att möta den ökande trenden nu när över hälften av alla internetköp görs via mobila enheter.

Mätningar har utförts på följande sidor:

- Startsida
- Kategorisida
- Produktsida"


Metod
-----------------------

Dessa verktyg har används för att mäta och samla data:

#### Google PageSpeed Insights

Denna användes för att undersöka prestandabetygen för webbplatserna och identifiera potentiella åtgärder för att påskynda sidans laddning.

#### Inbyggda Inspekt-verktyget i Webbläsaren (Chrome)

Uppladdningstider för DOM och total uppmättes tre gånger med hjälp av inspekt-verktyget. 

#### Google Sheets 

Det beräknade genomsnittsresultaten samlades i Google Sheets.

### Gräns för laddningstid:

Enligt Googles riktlinjer anses idealtiden ligga mellan 1-2 sekunder. Detta kan dock vara en optimistisk siffra, särskilt för e-handelssidor som behöver ladda in över 1000 artiklar. Personligen skulle jag hävda att en laddningstid på 3-4 sekunder fortfarande betraktas som relativt snabbt.

Resultat
-----------------------

<div class="gallery">
    <a href="%base_url%?image/kicksmobil.png" style="background-image:url(%base_url%?image/kicksmobil.png)">
    </a>
  <div class="desc"><h3>Bäst: Kicks</h3></div>
</div>

<div class="gallery">
    <a href="%base_url%?image/lykomobil.png" style="background-image:url(%base_url%?image/lykomobil.png)">
    </a>
  <div class="desc"><h3>Medioker: Lyko</h3></div>
</div>

<div class="gallery">
    <a href="%base_url%?image/bangerheadmobil.png" style="background-image:url(%base_url%?image/bangerheadmobil.png)">
    </a>
  <div class="desc"><h3>Sämst: Bangerhead</h3></div>
</div>

### Gemensamma Förbättringar

Enligt Google PageSpeed Insights finns det några enkla förbättringar som alla sidor kan genomföra redan idag för att bli snabbare:

- Fixa rätt storlek på bilder
- Minska oanvänd JavaScript
- Visa bilder i nästa generations format

För en mer långsiktig strategi, där maximal tidsbesparing är målet, kan följande åtgärder övervägas:

- Undvik en överdriven DOM-storlek
- Minska effekten av tredje parts kod
- Minska JavaScript-exekveringstiden

### Mätningar

<iframe class="google-sheets" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQQmqLR-7h27fBPYGm2ZnRGD2-iZ7wlP_5zWoEAaiD7VPLUDsPVDB39aL0R9b1apkLM4W1_UkDETkV0/pubhtml?widget=true&amp;headers=false"></iframe>


Samtliga butiker hade en genomsnittlig uppladdningstid över 5 sekunder för sina hemsidor, vilket överstiger den gräns jag ansett som önskvärd. Kicks presterade bäst genom att behålla samma laddningstid även på kategori- och produktsidorna. Å andra sidan ökade de andra två butikernas Page Load Average med ungefär 60%. Detta resultat var oväntat då jag hade förvänta mig att särskilt en ensam produktsida har färre element att ladda jämfört och därmed skulle va snabbare än framsidan.

Intressant nog visade det sig att Kicks, trots att de hade den sämsta laddningstiden på framsidan, hade bäst prestanda genom alla sidor genom att bibehålla samma tid. Bangerhead som hade bäst laddningstid på framsidan visade sig inte alls hålla måttet över hela hemsidan, vilket gjorde dem prestandamässigt sämst.

Personligen så upplever jag själv sidorna som snabbladdade när jag surfar på en padda eller mobil. Alla verkar ha lazy loading-feature som hjälper att ladda artiklarna allt eftersom de scrollas. Jag upplever heller inga direkt störningar eller långsamheter vid betalning. 

Analys
-----------------------

Resultatet visar att alla tre hemsidorna är ganska dåligt gjorda när det kommer till laddningstid och användarbarhet. Samtidigt är, särskilt butikssidor, ganska svåra att utveckla till snabba hemsidor. Alla butiker hade över 3000 element i sin DOM på framsidan. Bangerhead hade mest, med över 6000 element, vilket är nog grunden till att hemsidan inte höll måttet. Detta är möjligtvis något som skulle kunna ses över och skalas ner.

Några av de tricks som Shopifys artikel "Website Speed Optimization" går igenom är att man bör använda sig av quick view på kategorisidor. Detta är något Bangerhead faktiskt använder sig av, men detta verkar ändå inte ha hjälpt till mycket då betyget på en produktsida var så lågt som 14 sett utifrån PageSpeed Insights.

Som butik är produktbilder väldigt viktiga. En förbättring som dök upp på alla är att fixa rätt storlek på bilder. Ett annat tips av PageSpeed Insight var att använda sig av nästa generationens bild-format som WebP och AVIF istället för PNG och JPEG. De nya formaten erbjuder bättre kompression.

Överlag känns resultaten lite överdrivet dåliga. Dessa långsamma laddningstider upplevs knappt, särskilt när en sida väl blivit cashad till viss mån. Men att ha ett DOM-träd med över 6000 element känns inte heller hållbart och några av tipsen är ändå värda för företagen att se över.

Referenser
-----------------------

- [Trending up - Shopping on your phone](https://www.morningbrew.com/daily/stories/2023/11/26/record-online-shopping-fuels-another-massive-black-friday "Shopping on your phone")
- [Page Speed](https://moz.com/learn/seo/page-speed "Page Speed") 
- [Website Speed Optimization: 12 Techniques to Achieve Blazing-Fast Ecommerce Site Speed](https://www.shopify.com/enterprise/site-performance-page-speed-ecommerce#:~:text=Google%20recommends%20a%20page%20load,for%20your%20website%20to%20load. "Website Speed Optimization") 

Övrigt
-----------------------

Skriven av Isabel Salo