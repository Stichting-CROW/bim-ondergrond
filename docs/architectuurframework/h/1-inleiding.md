# Inleiding


## Aanleiding
CityDeal Openbare Ruimte heeft aan CROW gevraagd om te verkennen wat nodig is aan datastandaarden en afspraken om informatie over de ondergrond in de openbare ruimte van gemeenten beter te kunnen opstellen, beheren en publiceren. 
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



## Probleem
Vanuit bovenstaande context komt het Ontwikkelteam OT5 van de CityDeal Openbare Ruimte tot de vraag om "datastandaarden te verbinden". Het probleem is breed gedefinieerd, het betreft niet een of meerdere afgebakende use cases met een duidelijk werkproces, enkelvoudige informatiebehoefte, bekende informatiebronnen en applicaties, maar juist het hele samenspel van actoren en werkprocessen in de stedelijke openbare ruimte en infrastructuur die allemaal gebruik maken van de datastandaarden. Problemen van de datastandaarden, van de bestaande datasets, van de werkprocessen en van de systemen lopen door elkaar heen. Het kan in het geval van de datastandaarden gaan over de inhoudelijke aansluiting van de standaarden op elkaar, de technische aansluiting, de gebruikte talen en uitwisselformaten, de interpretatie door de gebruikers en systemen en nog veel meer. Waarbij iedere partij in het stedelijke gebied zelf bepaalt welke informatie wordt opgeslagen, en in welke standaard dat wordt uitgedrukt. Dat leidt tot het soort toepassingsvragen die in onderstaand voorbeeld zijn uitgelicht.

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
Het korte termijn doel van dit architectuur framework is een oplossing voorstellen waarvandaan de standaarden op elkaar kunnen worden aangepast. Daarbij zal gaandeweg blijken, of de gebruikers geholpen kunnen worden om hun informatiebehoefte beter te definiëren en of zij de informatie beter van elkaar kunnen overnemen. Dat lost nog niet meteen het vraagstuk op, hoe partijen hun informatie beter actueel en compleet kunnen houden en dit voor elkaar kunnen ontsluiten.

### Middellange termijn
De standaarden moeten waarschijnlijk verder worden uitgebreid om de volledige informatiebehoefte te dekken, dit zal verder moeten worden uitgewerkt in het BORius programma. 


## Doel document
Dit document beschrijft use-cases, inhoudelijke en technische uitgangspunten voor standaarden, toepassingsprofielen en uitwisselafspraken om de ondergrond goed in beeld te brengen. Met dit document geven we betrokken partijen (binnen en buiten de Citydeal) inzicht over een aanpak om data-standaarden over de ondergrond met elkaar te verbinden zodat deze in samenhang toegepast kunnen worden. Dit plan geeft uiteindelijk input aan de volgende fase die binnen het programma BORius zal worden opgepakt.

## Aanpak
Het probleem is breed gedefinieerd, het betreft niet een of meerdere afgebakende use cases met een duidelijk werkproces, enkelvoudige informatiebehoefte, bekende informatiebronnen en applicaties, maar juist het hele samenspel van actoren en werkprocessen in de stedelijke openbare ruimte en infrastructuur die allemaal gebruik maken van de datastandaarden. Daarom wordt gewerkt met een onderzoekende aanpak met de volgende stappen:

<ul><li>Met een groep modelleurs die het datavraagstuk goed kennen, samenwerken en bepalen welke objecttypen als eerste in een proefuitwerking moeten komen. Het gaat om de mensen die in hun dagelijks werk de pijn voelen van ontbrekende data bij integrale gebiedsvraagstukken, zoals ontwerpers of gebiedsplanners en de informatiekundigen die hen hierbij ondersteunen.</li>
<li>Proefuitwerkingen maken waarbij van één objecttype, bijvoorbeeld kademuren of kabels en leidingen, de datastandaarden op elkaar zijn afgestemd door het op dezelfde manier modelleren volgens de NEN 2660-2 en onderlinge verbanden leggen. Zie Figuur 3 Soorten informatie die op dezelfde manier gemodelleerd kunnen worden</li>
<li>Een praktijktoets te doen met die vertegenwoordigers of data gebaseerd op de beide standaarden onderling uitgewisseld kunnen worden. Hieruit kan dan blijken of<ul>
<li>Bestaande datasets actueel, betrouwbaar en compleet zijn</li>
<li>Bestaande datasets kunnen worden gepubliceerd voor toepassing in meerdere applicaties</li>
<li>Bestaande applicaties kunnen werken met data, die op de nieuwe manier gemodelleerd en gepubliceerd is</li>
<li>De overlap tussen datasets duidelijk wordt, zodat afgesproken kan worden wie de bronhouder is van welk deel van de informatie</li></li></ul></ul>

Dit resulteert in een voorstel waarin de datastandaarden beter op elkaar afgestemd zijn. Het vervolg (buiten scope van dit project) zal zijn om de wijzigingen op te nemen in de actuele versies van de standaarden, en een werkwijze af te spreken waarbij deze datastandaarden in samenhang beheerd kunnen worden, zodat de relaties actueel blijven bij updates. 


## Leeswijzer

Dit document beschrijft de volgende zaken: 

**2. Scope** beschrijft de scope van het probleem en de gezochte oplossingsrichtingen.

**3. Use case** beschrijft bij elke [=use case=] een weergave van het probleem, de stakeholders, het werkproces, de informatiebehoefte, de gebruikte systemen en de gewenste oplossingsrichtingen per use case.

**4. Technische uitgangspunten** beschrijft de technische uitgangspunten en eisen aan de informatiemodellen en andere datastandaarden die gebruikt worden in de boven- en ondergrondse openbare ruimte.

**5. Oplossingsrichtingen** beschrijft de technische oplossingsrichtingen die zijn uitgewerkt voor beproeving in de praktijk van de use cases.

**6. Praktijktoets** beschrijft uitgevoerde praktijkproeven en beoordeelt de praktische toepasbaarheid van de geboden oplossing.


**7. Aanbevelingen** In Aanbevelingen wordt een roadmap voor ontwikkeling van de datastandaarden in samenhang gegeven en worden randvoorwaarden beschreven voor de manier waarop de oplossingsrichtingen worden uitgewerkt samen met beheerders van standaarden en in interactie met gebruikers. 
