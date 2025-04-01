# Legacy-modernisering door heropbouwen

Software wordt vergelijken met de opbouwen van een huis, maar deze analogie schiet tekort: software evolueert continu.
Een tuin is een betere metafoor.
Sommige planten gedijen in de schaduw, andere in het zonlicht en insecten ("bugs") en onkruid moeten constant beheer worden.

Legacy-systemen worstelen vaak met performance, beveiliging, en privacy.
Het moderniseren van deze systemen door hedendaagse frameworks en programmeertalen te omarmen, kan helpen om deze uitdagingen aan te pakken.

In samenwerken met ShareValue kun je je zakelijke behoeften focussen, terwijl wij jouw IT-landschap 'tuineren'.

## Aandrijvende krachten

Er zijn twee manieren om "legacy" te bekijken:

- Negatief: ouderwets en verouderd
- Positief: een erfenis die heeft bijgedragen aan het succes van het verleden

Hoewel legacy-systemen misschien de basis waren voor de prestaties van een bedrijf, garandeert dit niet het toekomstige succes.
Positieve verandering wordt door actie gebracht.
Je kunt de toekomst niet voorspellen, maar de komende vijf jaar zullen net als de vorige vijf jaar zijn, tenzij er iets verandert.

Milieuveranderingen - veranderingen in de omgeving - vragen om aanpassing.
De gewassen hebben speciale omstandigheden nodig om te gedijen en boeren moeten die roteren om gezonde grond te beheren.
Evenzo moeten softwareontwikkelaars hun systemen evolueren om moderne omstandigheden te beheren, zoals opschalen en prestatieverbeteren.

Het is goedkoper om werknemers bij te scholen dan ze te verplaatsen, evanals de vernieuwing van huidige software praktischer dan deze opnieuw te bouwen.
Maar als er fundamenteel gebrekkige software is, zou opnieuw bouwen de enige optie zijn.

## Het landschap

De term "legacy-applicatie" doet je denken aan systemen uit de jaren '80, bijvoorbeeld die in C/C++, COBOL of Fortran werden geschreven.

Legacy-systemen vertonen vaak problemen:

- Observability: moeite met het analyseren van metrieken en logging
- Performance: trage opstart- en reactietijden
- Beveiligingsrisico's: kwetsbaarheden door onzorgvuldig geheugengebruik
- Platformafhankelijkheid: systemen die vastzitten aan verouderde hardware of software
- Hoge operationele kosten: leggen een zware last op het bedrijf
- Slechte onderhoudbaarheid: complexe, moeilijk te begrijpen code leidt tot trage ontwikkeling en oplossingen

## Moderne Platforms

Legacy-systemen die afhankelijk zijn van specifieke hardware (bijv. COBOL-systemen) moeten naar nieuwe platforms migreren, omdat die specifieke hardware wordt achterhaald door nieuwe innovaties.
Als de hardware niet meer wordt geproduceerd,heeft een bedrijf geen andere optie dan modernisering.

Java, Docker en Kubernetes gedijen dankzij hun platformonafhandkelijkheid, die een "write once, run anywhere" aanpak gefaciliteerd, kosten verlaagt en de onderhoudbaarheid vereenvoudigt.
Flexibiliteit stuwt ook de populariteit van Python, C# en JavaScript.

Veel industrieën, vooral bankwezen en de overheid, zijn afhankelijk van COBOL, maar gebruiken hun huidige ervaring met Java voor nieuwe systemen.
Technologiekeuzes zijn slechts één onderdeel van de puzzel.
Goed systeemontwerp, duidelijke documentatie en onderhoudbaarheid zijn belangrijker voor het vereenvoudigen van complexe legacy-processen.

Het provisioneren van omgevingen wordt geoptimaliseerd door cloudcomputing en tools zoals Bicep en Terraform.
Standaard-API's en verbeterde integraties versnellen de ontwikkeling, hoewel de complexiteit toeneemt door de interconnecties.

Het moderne landschap is niet alleen een tuin, maar een divers onderling verbonden bos: een ecosysteem.

## Noodzaak is de moeder van de uitvinding

Innovatie komt voort uit noodzaak.
Tijdens de COVID-19 pandemie moesten bedrijven zich snel aanpassen aan thuiswerken.
Net als een tuin gedijt wanneer deze gekoesterd wordt en zich aan veranderende omstandigheden aanpast, hebben softwaresystemen continue aandacht nodig.
Net als een goed onderhouden tuin die bloeit door zorg.

## Zaden zaaien

Om iets te verbeteren, moet je eerst bepaalde metingen verkrijgen.
Als je gelooft dat klanten gelukkig zijn, is het pas een overtuiging totdat het wordt bewezen door het ophalen van klantfeedback.
Je weet niet of een traag proces verbeterd kan worden totdat je de metingen van de snelheid kunt controleren.

Data-analyse is de sleutel tot het nemen van weloverwogen beslissingen.
Zonder data blijven ideëen en voorstellen subjectief.
Gebruik de wetenschappelijke methode: stel een hypothese op, voer een experiment uit, analyseer de resultaten en trek objectieve conclusies.

## Veldproeven en experimenten

Feedback kan aangeven dat je systeem of de teamreactietijden traag zijn.
Je kunt dit meten met verschillende testen:

- Prestaties: meet API-reactietijden en databasequerytijden
- UX: volg het aantal acties en wachttijden tijdens gebruikersactiviteiten
- A/B-test: verdeel gebruikers in twee groepen, A en B, met verschillende ervaringen, om tevredenhijd te meten
- Onderhoudbaarheid: analyseer metingen van de code (bijv. cyclomatische complexiteit)
- Beveliging: probeer bekende beveiligingsaanvalsmethoden om de systeemintegriteit te waarborgen en mogelijke kwetsbaarheden te identificeren

## Inzichten oogsten

Monitor interacties binnen je systemen.
Tools zoals [Hotjar](https://www.hotjar.com/product/heatmaps/) bieden heatmaps en sessie-opnames, terwijl [Google Analytics Events](https://developers.google.com/analytics/devguides/collection/ga4/events) gebruikersacties kunnen volgen.
In het geval van privacyzorgen bij gebruikers, kunnen deze activiteiten binnen een controlegroep worden uitgevoerd.
Het implementeren van experimenten zoals A/B-testen stelt je in staat om objectieve feedback over systeemverbeteringen te verkrijgen.

## Barometers en regenmeters

Milieumetingen begeleiden de groei van een tuin, net zoals observability software-prestatie-optimalisatie kan begeleiden.
De API-prestaties van verschillende scenario's kunnen worden gemeten met tools zoals [Apache JMeter](https://jmeter.apache.org/) of [Grafana k6](https://k6.io/) via [verschillende loadtests](https://grafana.com/docs/k6/latest/testing-guides/test-types/#different-tests-for-different-goals) om deze scenario's in je systeem te simuleren.

- **Smoke tests:** Minimale belasting
- **Gemiddelde-load tests:** Normale omstandigheden
- **Soak tests:** Betrouwbaarheid over langere perioden
- **Stress tests:** Het systeem tot zijn grenzen duwen
- **Spike tests:** Korte, massale pieken in activiteit
- **Breakpoint tests:** Het vinden van het breekpunt

Het analyseren van de applicatie- en systeemlogboeken over bepaalde periodes kan waardevolle inzichten opleveren, vooral met technieken zoals gestructureerde logging vanuit frameworks zoals [NLog](https://nlog-project.org/) of [Serilog](https://serilog.net/) in .NET.
Er zijn verschillende leveranciers die geavanceerde analyseproducten aanbieden op basis van verzamelde gegevens:

- [Azure Monitor](https://learn.microsoft.com/en-us/azure/azure-monitor/) met [Azure Application Insights](https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview)
- [Splunk](https://www.splunk.com/en_us/products/observability.html)
- [DataDog](https://www.datadoghq.com/product/observability-pipelines/)

De juiste loadtest kan gebruikersfeedback verifiëren, bijvoorbeeld het ervaren van pieken in belasting of een gestrest systeem kan leiden tot timeouts.
Opschalen tijdens hoge vraag en daarna weer afschalen kan helpen om prestaties en kosten in balans te houden.
Proactieve monitoring en observability zouden mogelijk het probleem kunnen verhelpen voordat klanten de systeemdegradatie opmerken.
Geavanceerde analyse van gebruikersgedrag kan zelfs pogingen van kwaadwillende gebruikers identificeren om beveiligingsaanvallen uit te voeren.

## Houd de vossen en bugs buiten

Een boer beschermt zijn vee tegen de jacht door vossen.
Een tuinier probeert insectenplaag te vermijden die zijn gewassen kunnen vernietigen.

Legacy-systemen zijn bijzonder kwetsbaar voor beveiligingsrisico's, aangezien verouderde frameworks en talen een doelwit zijn voor cyberaanvallen.
Moderne programmeertalen zoals Kotlin, Rust en C# helpen deze uitdagingen aan te pakken door zich te concentreren op veiligheid en het minimaliseren van veelvoorkomende fouten, waardoor kwetsbaarheden die vaak in oudere systemen te vinden zijn, worden voorkomen.

Nieuwere versies van C# (vanaf C# 8.0) introduceren nullable reference types, die null reference exceptions kunnen voorkomen, een veelvoorkomende oorzaak van runtime-fouten die de code moeilijk te debuggen en te onderhouden maken.
Voor observability- en operationele teams kunnen deze uitzonderingen logs vervuilen en de root cause-analyse bemoeilijken.
Moderne C# vermindert het risico op deze problemen, wat de beveiliging, onderhoudbaarheid en operationele efficiëntie verbetert.

Kotlin biedt vergelijkbare voordelen met betrekking tot null-veiligheid.
Daarnaast maakt de beknopte syntax van Kotlin, verbeterde gelijktijdigheidsbehandeling en sterke integratie met Java het een uitstekende keuze voor het moderniseren van Java-gebaseerde systemen.
Dit vermindert de risico's die gepaard gaan met foutgevoelige code, terwijl de codekwaliteit wordt verbeterd.

Rust legt de nadruk op geheugensveiligheid zonder een garbage collector.
Het voorkomt problemen zoals buffer overflows, geheugenlekken en dangling pointers tijdens de compileertijd.
Dit helpt om high-performance systemen veilig en betrouwbaar te houden, wat vooral belangrijk is in beveiligingskritieke omgevingen zoals blockchain en IoT.
Rust's strikte eigendomregels en geheugenbeheer tijdens compileertijd helpen veel kwetsbaarheden te verminderen die vaak voorkomen in oudere systeemprogrammeer-talen zoals C en C++.

Door de nieuwste functies van moderne programmeertalen te adopteren, kunnen bedrijven beveiligingskwetsbaarheden aanzienlijk verminderen, het systeemonderhoud stroomlijnen en de algehele observability verbeteren, wat resulteert in meer veilige, onderhoudbare en toekomstbestendige systemen.
En misschien wel gelukkigere ontwikkelingsteams.

## Snoeien en Onderhoud

Bloeiende wijnranken en andere klimplanten zijn prachtig om naar te kijken, totdat ze uit de hand lopen.
Ze kunnen andere planten verstikken en zelfs de muren van gebouwen beschadigen waar ze zich aan vastklampen.
Regelmatig snoeien is nodig om de balans te behouden en een verwarde puinhoop te vermijden.

Hetzelfde geldt voor softwarecode.
Tools kunnen helpen bij het beheren van de groeiende softwarewouden:

- Cyclomatische complexiteit om de complexiteit te minimaliseren
- Unit test code coverage rapporten om te zien hoeveel is gedekt door veiligheidsnetten voor correctheid
- Statische analysetools zoals EditorConfig, Checkstyle, SonarQube, eslint en anderen zorgen voor standaardisatie en consistentie

Een andere interessante tool is [CodeCharta](https://codecharta.com/docs/analysis/metrics), die een codebase visualiseert als een stadskaart.
Het hebben van een tastbaardere weergave helpt bij het spotten van problematische gebieden, zoals codegebieden met constant hoge code-churn, of gebieden die mogelijk kennisgaten hebben door gebrek aan teamexposure.

Er zijn enkele wetten die hier in gedachten gehouden kunnen worden, zoals de Wet van Afnemende Opbrengsten, Brooke's Law, Amdahl's Law en Goodhart's Law: Wanneer een metric een doel wordt, stopt het met een goede metric te zijn.
Na een bepaald punt leveren extra inspanningen om onderhoudbaarheid te verbeteren weinig waarde op, dus wees voorzichtig met het investeren van focus en extra middelen als deze contraproductief worden.

## Beheerde Ecosystemen of Wilde Jungles

Software systemen automatiseren bedrijfsprocessen.
Vroeger was het overmaken van geld tussen bankrekeningen een taak voor een klerk, maar tegenwoordig gebeurt dit via een mobiele app.

Bedrijfsregels, beleidsmaatregelen en wetten vormen de basis van een softwaresysteem.
Conway's Law suggereert dat het ontwerp van de software van een organisatie vaak de communicatie structuren weerspiegelt.
Het vereenvoudigen van software vereist daarom vaak het vereenvoudigen van de onderliggende bedrijfsprocessen.

Tenslotte, software is een erfenis, maar de waarde die een bedrijf brengt is zijn erfgoed.

## Zorggidsen

Onderhoudbaarheid gaat niet alleen over code; het omvat ook documentatie.
Het begrijpen van hoe een proces werkt en het vastleggen van die kennis is essentieel voor het bedrijf.
Tools zoals Markdown, Asciidoc, Confluence en SharePoint kunnen helpen bij het beheren van deze kennis en bedrijfscontinuïteit.

Zelfs hier kunnen metrics helpen.
Tools die gemiddelde leestijden voor documenten berekenen, zoals het gebruik van [Medium's leestijd](https://help.medium.com/hc/en-us/articles/214991667-Read-time) algoritme, kunnen de betrokkenheid van lezers bij je documentatie verbeteren.

## Jouw Betrouwbare Tuinservice: ShareValue

Het moderniseren van legacy-systemen kan voelen als het onderhouden van een complex ecosysteem, waarbij constante zorg en expertise nodig zijn.
In plaats van je tuinen zelf te verzorgen, fungeert ShareValue als jouw vertrouwde tuinservice, die de juiste tools, kennis en ervaring biedt om je softwaresystemen te verzorgen.

Van het beoordelen van je huidige landschap tot het bieden van doorlopend onderhoud, zorgen wij ervoor dat je systemen veilig, schaalbaar en klaar voor de toekomst blijven, zodat jij je kunt concentreren op wat echt belangrijk is: je bedrijf laten groeien en een erfenis van waarde achterlaten.
