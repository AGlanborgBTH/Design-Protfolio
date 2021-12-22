---
Title: Load
Description: The time it takes to load sites
Template: reports
---
Loading time
=======================

Mängden webbsidor på internet växer varje dag och tävligen för användarens uppmärksamhet mellan alla webbsidor blir hårdare och hårdare. Så nu är det viktigare än någonsin att optimera alla webbsidor för att hamna före alla andra, och det innebär snabbare laddnings-tider.

Urval
-----------------------

Valet av webbplatser för denna undersökning var: Ica, Willys och Coop.  
Motiveringen till dessa val av webbplatser var Online-handel. Sen Corona-pandemin startade så har efterfrågan för Online-shopping blivit mycket större. Matbutiker är en av de typer av affärer som har ändrats mest. Under Corona så har det blivit mycket vanligare med hemleverans och upphämting av färdig-samlade produkter. Till skillnad från (t.ex.) klädaffärer så har mat-butiker inte haft någon längre historik med Online-handel, så är det en enorm skillnad från mat-affärers tidigare affärsplaner.  
Eftersom de inte har en längre historik av internet-handel och eftersom efterfrågan är så hög, så är det viktigt att deras hemsidor anpassas och uppdaterars för bättre upplevelser för konsumenter.

Metod
-----------------------

Anteckna datum och besök de tre följande hemsidorna i webb-browsern Chrome:
1. [https://www.ica.se](https://www.ica.se)
2. [https://www.willys.se](https://www.willys.se)
3. [https://www.coop.se](https://www.coop.se)

På varje sida sen:
- Öppna Chromes Network-tab i Developer Tools meny och anteckna hemsidans laddningstid, antalet hämtade filer och den totala storleken på alla hämtade resurser, efter att "disable cache" är aktiverat och ctrl+shit+r trycks. Gö allt tre gånger och sedan anteckna medianen av alla värden.
- Öppna Google Pagespeed och länka sidan, sedan anteckna informationen, relaterat till laddningstider, som den ger. Gö det för både Mobil och Dator. 

Resultat
-----------------------

### ICA

<div class="imgrow">
    <div class="reportimg">
        <a href="%assets_url%/img/ica.PNG" target="_blank">
            <picture>
                <source srcset="%assets_url%/img/ica1.png" media="(min-width: 769px)">
                <source srcset="%assets_url%/img/ica2.png" media="(max-width: 768px)">
                <img src="%assets_url%/img/ica.PNG" alt="https://www.ica.se" title="ICA 12/12/2021">
            </picture>
        </a>
    </div>
</div>

### Willys

<div class="imgrow">
    <div class="reportimg">
        <a href="%assets_url%/img/willys.PNG" target="_blank">
            <picture>
                <source srcset="%assets_url%/img/willys1.png" media="(min-width: 769px)">
                <source srcset="%assets_url%/img/willys2.png" media="(max-width: 768px)">
                <img src="%assets_url%/img/willys.PNG" alt="https://www.willys.se" title="Willys 14/12/2021">
            </picture>
        </a>
    </div>
</div>

### Coop

<div class="imgrow">
    <div class="reportimg">
        <a href="%assets_url%/img/coop.PNG" target="_blank">
            <picture>
                <source srcset="%assets_url%/img/coop1.png" media="(min-width: 769px)">
                <source srcset="%assets_url%/img/coop2.png" media="(max-width: 768px)">
                <img src="%assets_url%/img/coop.PNG" alt="https://www.coop.se" title="Coop 12/12/2021">
            </picture>
        </a>
    </div>
</div>

### Prestation

<iframe class="sheet" title="Prestation resultat" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSahQdX7XQe53ivH7f12IAmmB9kavN1f5gJUGZQVFCNgRjZy3nbGnBP4vVmm9Vpvsr-EcvnEppiDPsT/pubhtml?widget=true&amp;headers=false"></iframe>

Analys
-----------------------

Efter dagens standard så är ingen av sidorna bra gjord. De tar lång tid att ladda och kräver användaren att ladda hem mycket data för att vara en sida. Det är förväntat att en sida ska ta mellan 1 och 3 sekunder att ladda (vilket endast Willys hemsida uppnår) och att användaren hämtar runt 1MB data för en sida. Dock angående det later, eftersom dessa sidorna är riktade mot Svenska personer så är det inte lika relevant som det en gång var. Dagens Svensk har tillgång till mer och snabbare internet idag än vad de hade för 5 år sedan. Dessutom är de hemsidor för matprodukter och förväntas ha bilder på deras produker, men det argumentet är inte relevant sen det är inte heller förväntat att de visa upp produkter på deras första sida.

Den sidan som stack ut mest av alla tre sidor var ICA. ICAs sida hade få filer med en mindre total bit-storlek än de andra två sidorna, men de hade nästan lika lång laddningstid som Coop (som hade flest filer). Anledningen till detta kan vara för att de har någon extra stor fil som de hämtar. För de hämtar totalt 69 filer som tar upp 1.63MB när de är compressed, men sen när de packar upp filerna så når de 5.6MB. Filerna blir 4 gånger så stora efter att webbläsaren öppnar dem. Det kan även förklara varför det tar 3.4s för alla DOM-element att ladda klart på sidan. Fast Ica har en sida som inte är fullt optimerad för datorer, så är deras sida värre för mobiler. Enligt [Page Speed](https://pagespeed.web.dev/) så tar det 13.4 sekunder innan man kan interagera med sidan. Från endast den siffran och dens innebörd dras slutsatsen att ICAs hemsida är inte gjord för mobiler. Det antas att ICA satsar på att göra en app för mobilanvändre istället för en optimerad hemsida. Men att förvänta sig att alla som söker sidan kommer ladda ner appen är ignorant. ICA bör optimera eller göra om deras hemsida, för både datorer och mobiler. Det är förväntat att sidor laddar snabbare än vad det gör för ICA idag.

Willys hemsida var den mest optimerade sidan av de tre utvalda sidorna. De hade en laddningstid på 2.5 sekunder och nedladdade filer med den totala storleken av 1.9MB. Willys hemsida för datorer är väl optimerad, men när det kommer till mobiler sen så faller den för samma sak som ICA gör. [Willys.se](https://www.willys.se/) tar 14.4 sekunder innan de går att interagera med. Det antas de inte optimerar sidan av samma anledning att ICA inte optimerar deras sida för mobilanvändare: Willys har en app som de vill att mobilanvänder använder. Persis som ICA så bör Willys optimera sin sida eller göra om den för att göra det bättre för mobilanvändare. Alla användare som kommer deras sidor kommer inte ladda ner appen, så de bör optimera sidorna för de användarna.

Coop hade den största sidan av de tre utvalda sidorna. De krävde 3.5MB av nedladdad data, utspritt över 187 unika filer för att användare ska använda sida. Det är Välldigt mycket data då det är förväntat att sidor endast ska kräva ca. 1MB nedladdad data. Dock laddar sidan välldigt snabbt. När de nedladdade filerna öppnas expanderas de och når 7.3MB, men ändå laddas hela sidan klart på 5.7 sekunder. 5.7 sekunder är lång tid enligt dagens standard, men för att ha så många filer med så mycket total data så är det välldigt snabbt. Vad de skulle kunna göra för att optimera sidan är att minimera mängden filer hämtade. Om de skulle ta bort filer och tog bort onödig kod så skulle sidan laddas snabbare för både datorer och mobiler.

Coops hemsida är inte gjord för mobiler. Coops hemsida tar längst tid att ladda av alla tre sidor, på mobiler, med tiden 16.6 sekunder innan användare kan använda sidan. Presis som de andra två sidorna så är det mest troligen för att de har en app som de vill att användare ska använda. Men precis som de andra två sidorna så missar de potentiella kunder som inte vill vänta på att sidan laddar varje gång de trycker på någon länk. Därför bör de optimera eller göra om sidan så att de blir mera mobil-vänliga.

Om laddningstider inte räknas med så var ICAs hemsida bäst gjord, och har mest potential. Det är eftersom deras startsida består av länkar till olika artiklar och andra delar av hemsidan, och inga produkter visas direkt till användaren på första sidan. Det är för att varje ICA butik har olika priser och kan inte visa upp deras "veckans priser" direkt på startsidan utan att specifisera vilken butik som diskuteras. Anledningen till att det är en possitiv sak är för att det har potentialen att minimera mängden hämtad data, då de inte använder lika många bilder som både Willys och Coop gör på deras startsida. Vad Willys och Coop skulle kunna göra för att optimera deras sidor är att följa ICAs exempel. Mindre biler och/eller optimerade bilder för att minimera laddningstiden, och även specifisera höjd och storlek på varje bild (vilket ICA inte gjorde). Om Willys och Coop gör om sina startsidor så kommer de nå bättre laddningstider för både Dator och Mobil. ICA bör optimera deras hemsida och göra den bättre för både dator- och mobil-användare.

I en lista av dessa tre sidor från best gjord sida till sämst gjord sida så skulle listan se ut som följande:
1. Willys
2. Coop
3. ICA

Referenser
-----------------------

ICA. (2021). *ICA*. Hämtad december 12, 2021 från [https://www.ica.se/](https://www.ica.se/)

Willys. (2021). *Willys*. Hämtad december 12, 2021 från [https://www.willys.se/](https://www.willys.se/)

Coop. (2021). *Coop*. Hämtad december 12, 2021 från [https://www.coop.se/](https://www.coop.se/)

Övrigt
-----------------------

Skriven av: Anton Glanborg

14/12-2021
