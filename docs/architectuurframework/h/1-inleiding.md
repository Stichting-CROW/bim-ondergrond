# Inleiding


## Aanleiding
De CityDeal Openbare Ruimte [externe link](https://www.citydealopenbareruimte.nl/default.aspx) heeft aan CROW gevraagd om te verkennen wat nodig is aan datastandaarden en afspraken om informatie over de ondergrond in de openbare ruimte van gemeenten beter te kunnen opstellen, beheren en publiceren. 
Uitgangspunt hierbij is werken op basis van gebiedscasussen, liefst met een verschillende schaal, verschillende problematiek en met grote en middelgrote gemeenten. De CityDeal omarmt de ontwikkelingen van BORius waarbinnen dit projectvoorstel past en wil met haar bijdrage voor dit project een impuls geven aan BORius. Hiervoor werken de deelnemende gemeenten nauw samen om de bevindingen en resultaten in de gemeentelijke praktijk te beproeven en toe te passen.

<figure>
<img src="./h/media/gebiedscasussencitydeal.png" alt="Gebiedscasussen uit de CityDeal: Tilburg: Klimaatmaatregelen binnenstand; Amersfoort: Verbeerd programma openbare ruimte; Zoetermeer: Meerzicht, integrale wijkaanpak; Amstyerdam: Wallengebied, integrale ontwerpaanpak">
<figcaption>Gebiedscasussen uit de CityDeal</caption>
</figure> 


## Context
Met alle maatschappelijke opgaven als energietransitie, klimaat adaptatie, diverse vervangingsopgaven (bestaande ondergrondse netwerken, kademuren, riolering etc) en het streven naar een gezonde en leefbare stad met een goede bodem en (grond)waterkwaliteit, is het steeds meer een puzzel om in de ondergrond alles passend te krijgen. Een voorbeeld: ruimte maken voor parkeervakken in het heden, kan betekenen dat men in de ondergrond straks geen ruimte meer heeft voor de voorzieningen die nodig zijn voor de energietransitie. Daarom moeten oplossingen intergaal worden ontwikkeld. Hiervoor is goede informatie nodig over de functies en het ruimtegebruik in de ondergrond. De informatie over de ondergrond wordt geproduceerd en beheerd door verschillende partijen. Bij het overwegen van aanpassingen aan de openbare ruimte is informatie over de bestaande situatie en gewenste toekomstige functionaliteiten versnipperd en niet-samenhangend beschikbaar. De gevolgen van keuzes zijn daarom niet altijd zichtbaar. Het zou een doorbraak zijn als verschillende tools op ieder moment de beschikbare informatie over de ondergrond zouden kunnen raadplegen en ontsluiten. Met daarbij als uitgangspunt dat data-eigenaren controle houden over hun eigen data en in hun eigen bedrijfsomgeving kunnen blijven werken. 

<figure>
<img src="./h/media/soorteninformatie.png" alt="Verschillende soorten informatie: Beheerinformatie (conditiemetingen, materiaalkosten), kwaliteitsinformatie (besluiten, eisen, verificatie, validatie), meetinformatie (x,y,z, meetonnauwkeurigheid), ontwerp en bouw (2D, 3D, parameters, analyses), Stuurinformatie (kosten, presntaties, risico's)">
<figcaption>Verschillende soorten informatie over het stedelijk gebied</caption>
</figure> 


### BORius
Het Programma BORius is een initiatief van CROW en Stichting Rioned. De hoofddoelstelling: “In 2030 beschikken Assetmanagers en hun (keten)partners in de openbare ruimte en infrastructuur over een samenhangend stelsel objectstandaarden in de leefomgeving om de data over hun beheerde assets efficiënt op orde te houden en uit te wisselen”. De onderliggende doelstellingen van het programma zijn: 
* Logische informatiestructuur: Beter samenhangende informatiemodellen voor alle beheerde assets in de Openbare Ruimte en Infrastructuur
* Uitwisselproces: Op meer gestandaardiseerde manier data delen in de keten voor eenduidige interpretatie
* Samenhang, adoptie, en beheer: Meer actuele standaarden en werkwijzen voor informatieuitwisseling in de keten

## Vraagstelling vanuit CityDeal
Vanuit bovenstaande context komt het Ontwikkelteam OT5 van de CityDeal Openbare Ruimte tot deze vragen: 
* Hoe ondersteunen de huidige datastandaarden een datagedreven integrale aanpak? Sturing op “vitale systemen” wordt steeds belangrijker. ("Is er een probleem?")
* In welke richting en hoe kunnen datastandaarden in samenhang ontwikkeld worden? Zijn er bijvoorbeeld aanpassingen nodig (bv over planning) aan de data-standaarden om de tactische ruimte tussen strategische afstemming (stedelijk programmeren) en uitvoering te overbruggen? Zijn de data-standaarden ook bruikbaar in het stedelijke ontwikkelproces van initiatief-plan-ontwerp-uitvoering of zijn het toch vooral instrumemten voor asset-beheer? ("Welke oplossingsrichtingen zijn er bij het probleem?)
* Hoe belangrijk is het daarbij dat data-standaarden in samenhang worden doorontwikkeld (of hoe belangrijk is BORius voor het integraal werken). ("Lossen deze oplossingsrichtingen het probleem op?")


## Probleem
De huidige werkwijze leidt tot fragmentatie in data, waarbij het in samenhang bevragen van de data een puzzel is. 
Ook moet een databeheerder data naar verschillende bronnen sturen, en zelf de puzzel maken hoe deze bronnen met ongelijksoortige standaardenm

In het onderstaande voorbeeld worden voorbeelden gegeven van dit probleem.

<aside class="note" title="Standaarden als puzzelstukjes">
“Een gemeente die informatie vastlegt over een stroomkabel bij een lichtmast, gebruikt daarvoor IMBOR. De daarnaast liggende stroomkabel is door een netbeheerder vvastgelegd volgens IMKL. Als we een integrale kaart maken met daarop de objecten in de ondergrond, zien we bij de ene kabel heel andere informatie dan bij de andere. Dit leidt tot verwarring bij de gebruikers van de informatie”<br>
<br>
“In IMGeo staat een andere definitie van een boom dan in IMBOR, maar het model vertelt me semantisch dat ze hetzelfde zijn, wat moet ik nu aanhouden?” <br>
<br>
“In IMBOR staan kunstwerken beschreven vanuit een beheer-perspectief; hoe combineer ik dat nu met de decompositie vanuit de NEN 2767 die de kunstwerken bekijkt vanuit conditiemetings-perspectief?”<br>
<br>
“Ik heb een ontwerp gemaakt in AutoCAD, met NLCS. Nu moet ik voor de beheerder de informatie aanleveren in GIS, volgens IMGeo en IMBOR. Hoe transformeer ik dat zo efficiënt mogelijk?” <br>
</aside>

<figure>
<img src="./h/media/standaarden.png" alt="Ongelijksoortige standaarden (fruit, vervoermiddelen) bij de verschillende soorten informatie: Beheerinformatie (conditiemetingen, materiaalkosten), kwaliteitsinformatie (besluiten, eisen, verificatie, validatie), meetinformatie (x,y,z, meetonnauwkeurigheid), ontwerp en bouw (2D, 3D, parameters, analyses), Stuurinformatie (kosten, presntaties, risico's)">
<figcaption>Ongelijksoortige standaarden bij de verschillende soorten informatie over het stedelijk gebied</caption>
</figure> 


##	Doel, nut en waarde

### Korte termijn
Het korte termijn doel van dit project is laten zien in een showcase, hoe het op elkaar aansluiten van standaarden kan helpen bij het gebruik van data over de openbare ruimte en infrastructuur. 

### Middellange termijn
De standaarden moeten waarschijnlijk verder worden uitgebreid om de volledige informatiebehoefte te dekken, dit zal verder moeten worden uitgewerkt in het BORius programma. 


## Doel document
Dit document beschrijft use-cases, inhoudelijke en technische uitgangspunten voor standaarden, toepassingsprofielen en uitwisselafspraken om de ondergrond goed in beeld te brengen. Met dit document geven we betrokken partijen (binnen en buiten de Citydeal) inzicht over een aanpak om data-standaarden over de ondergrond met elkaar te verbinden zodat deze in samenhang toegepast kunnen worden. Dit plan geeft uiteindelijk input aan de volgende fase die binnen het programma BORius zal worden opgepakt.

## Aanpak
In eerste instantie was een aanpak geformuleerd, waarbij met databeheerders zou worden samengewerkt bij het uitwerken van use cases. Gezien de beperkte beschikbaarheid van dergelijke professionals, die hard nodig zijn voor operationele taken, is besloten om CROW de beschikking te geven over datasets waarmee een showcase gemaakt kon worden. CROW heeft:

* Datasets getransformeerd naar linked data
* Relaties gelegd tussen de gebruikte informatiemodellen 
* Laten zien dat je door deze relaties queries kan uitvoeren over meerdere datasets



## Leeswijzer

Dit document beschrijft de volgende zaken: 

**3. Use case** beschrijft uses cases met een weergave van het probleem, de stakeholders, het werkproces en de informatiebehoefte. 

**4. Technische uitgangspunten** beschrijft de technische uitgangspunten en eisen aan de informatiemodellen en andere datastandaarden die gebruikt worden in de boven- en ondergrondse openbare ruimte.

**5. Aanbevelingen** In Aanbevelingen wordt een roadmap voor ontwikkeling van de datastandaarden in samenhang gegeven en worden randvoorwaarden beschreven voor de manier waarop de oplossingsrichtingen worden uitgewerkt samen met beheerders van standaarden en in interactie met gebruikers. 
