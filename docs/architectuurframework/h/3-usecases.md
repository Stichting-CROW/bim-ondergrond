# Use Cases 

## Definitie use case

<dfn data-lt="Use case">Use case</dfn>
<dd>Beschrijving van een systeem vanuit het gebruikersperspectief, met een actor, de initiator van de interactie, en het systeem zelf als een opeenvolging van eenvoudige stappen. […] Actoren kunnen eindgebruikers, andere systemen of hardware (apparatuur) zijn. Elke usecase is een complete serie van zogenaamde "events", beschreven vanuit het standpunt van de actor. Bron: <a href="https://nl.wikipedia.org/wiki/Usecase">Wikipedia</a></dd>

<figure>
<img src="./h/media/werkwijzeusecases.png" alt="Visualisatie hoe vanuit een use case met werkproces, informatiebehoefte en gebruikte systemen gewerkt kan worden aan het afspreken van datapakketjes die worden uitgewisseld tussen landelijke voorzieningen, in de beheerorganisaties, in de projectorganisaties en met opdrachtnemers in het stedelijke gebied">
<figcaption>De opgave voor partijen die werken in het stedelijke gebied: Van use case naar begrijpelijke datapakketjes</caption>
</figure>


## Casus Wallengebied

We hebben de casus onderzocht van "principe-ontwerpen van toekomstige ondergronde infrastructuur in het Wallengebied" en daarbij het volgende gezien:
* **Use case 1** De ontwerper wil de bestaande ligging van ondergrondse objecten en relevante bovengrondse objecten in kaart brengen;
* **Use case 2** De ontwerper wil weten wat de eisen en parameters zijn bij het ontwerpen van een nieuwe situatie;
* **Use case 3** De ontwerper wil weten welke ondergronds objecten aanwezig moeten zijn in de nieuwe situatie: input vanuit beleid en de planfase. 
* **Use case 4** De ontwerper wil principeprofielen maken voor de inrichting van de ondergrond van een straat met aan één zijde gebouwen en aan de andere zijde een gracht en daarbij de afwegingen weergeven bij het ontwerp, zoals afwijking van de eisen over afstanden tot andere objecten omdat er niet voldoende ruimte is.
* **Use case 5** De ontwerper wil aangeven welke variabelen leiden tot welk principeprofiel, zodat er een onderbouwde afweging gemaakt kan worden voor het te kiezen principeprofiel bij elke straat.

### Hoog over scenario riolering / bor

* Uitwisseling tussen twee systemen die de integratie van rioleringsgegevens vereist in een <abbr title="Beheer Openbare Ruimte">BOR</abbr>-systeem (het ene systeem is conform IMBOR ingedeeld, het andere systeem conform een interpretatie van de GWSW-ontologie)
* Uitwisseling tussen twee systemen die de integratie van BOR-gegevens vereist in een rioleringssysteem (bijv. verhardingen, wadi's, meubilair) (het ene systeem is conform IMBOR ingedeeld, het andere systeem conform een interpretatie van de GWSW-ontologie)
* GWSW-dataset uitwisselen vanuit een integraal beheersysteem dat conform IMBOR is ingedeeld (bijv. hoe kom je van IMBOR naar .orox)
* IMBOR als standaard gebruiken voor vaste objectgegevens, maar daar GWSW-dynamische gegevens bij willen registreren
* Gegevens van aannemer die volgens GWSW kan inspecteren/etc. opnemen in beheersysteem conform IMBOR

In een gemeente kan het best zo zijn dat Assetmanager Riolering een applicatie voor Riolering gebruikt en andere Assetmanagers een integraal systeem. Die eerste Assetmanager moet dan ofwel data aan de anderen leveren voor het integrale beeld (situatie 1); ofwel data ontvangen van de anderen voor het verkrijgen van overzicht/bepaalde berekeningen (situatie 2)



## Use case 1: in kaart brengen bestaande situatie 

Use Case 1: In samenhang bevragen van data om het bestaande ondergrondse ruimtegebruik in kaart te brengen.

### Doelstelling

Het combineren van de gegevens gestructureerd via GWSW/IMBOR/IMKL/IMGeo, om een zo volledige mogelijk beeld van het ondergrondse ruimtegebruik te krijgen.

### Actoren

#### Gebruikers

* Databeheerders
* Ontwerpers binnen een integraal project van een gemeente

### Beschrijving

#### Stap 1: Verzamelen datasets
De ontwerper verzoekt de beheerders van de assets om de datasets die nodig zijn voor het in kaart brengen van de bestaande situatie aan te leveren. Deze datasets zijn gebaseerd op de open standaarden IMBOR, IMKL, IMGeo en GWSW (en meer?)

* Uit het Rioleringsysteem moeten type, liggings- en dimensiegegevens komen van een representatief aantal objecten;
* Uit het BORsysteem moeten type, liggings- en dimensiegegevens komen van een representatief aantal objecten;
* Uit de systemen van Netbeheerders en het Kadaster (Klik) de liggingssgegevens van bestaande kabels en leidingen.
* Alle datasets zijn als RDF beschikbaar en geclassificeerd aan respectievelijk GWSW en IMBOR en andere standaarden.


#### Stap 2: Verwerken datasets
De ontwerper verwerkt de aangeleverde datasets in het ontwerpproces. Hierbij worden de datasets geanalyseerd en omgezet naar een bruikbaar format.
* Middels de alignment die gemaakt is tussen standaarden worden conclusies getrokken over welke objecten hetzelfde zijn en zodoende welke gegevens gecombineerd kunnen worden;
* Deze 'nieuwe' gegevenset wordt beschikbaar gemaakt in een (visueel) systeem;
* De gebruiker gebruikt de gecombineerde gegevens om het ondergrondse ruimtegebruik in kaart te hebben.

#### Stap 3: Onderzoeken compleetheid en informatie
Voordat de ontwerper aan de slag gaat met de verwerkte datasets, wordt onderzocht of de datasets compleet zijn en voldoende informatie bevatten om mee te kunnen werken.

#### Stap 4: In kaart brengen bestaande situatie
Met behulp van de verwerkte datasets en eventueel aangevuld met eigen metingen, brengt de ontwerper de bestaande situatie in kaart.

#### Alternatieve scenario's

* Als de gegevens niet correct worden gecombineerd, kan het zijn dat het volledige ondergrondse ruimtegebruik niet correct wordt weergegeven. In dat geval moet de gebruiker de gegevens opnieuw combineren of de fout corrigeren.
* Als er wijzigingen worden aangebracht in de beiden datsets, moeten de gegevens opnieuw worden geëxporteerd en gecombineerd om het volledige ondergrondse ruimtegebruik up-to-date te houden.


### Data bestaande situatie
#### Bomen
De ontwerper heeft de volgende input nodig vanuit de assetbeheerder / bestaande situatie:
* Welke gegevens zijn nodig om bij het ontwerpen rekening te kunnen houden met  de bestaande bomen?
 Welke gegevens zijn bekend bij de beheerder van de openbare ruimte?
* Welke informatiemodellen worden gebruikt door deze beheerder?
* Dekken deze informatiemodellen de informatiebehoefte af?


#### Rioleringen
De ontwerper heeft de volgende input nodig vanuit de assetbeheerder / bestaande situatie
* Welke gegevens zijn nodig om bij het ontwerpen rekening te kunnen houden met de bestaande riolering?
* Wat zijn de maten en ligging van de riolering?
* Welke gegevens zijn bekend bij de beheerder van de riolering?
* Welke informatiemodellen worden gebruikt door deze beheerder? IMBOR en GWSW?
* Dekken deze informatiemodellen de informatiebehoefte af?
* Wat voor objecten liggen er boven de uit te graven/te vervangen riolering?
*  Wat is het afgekoppelde oppervlak?
*  Zijn de afwateringsvoorzieningen voldoende voor dit verharde gebied?
*  Wat is de doorstroming van het oppervlaktewatersysteem?
*  Wat is de bergingscapaciteit van het oppervlaktewatersysteem?



#### Electriciteitskabels
De ontwerper heeft de volgende input nodig vanuit de assetbeheerder / bestaande situatie

* Welke gegevens zijn nodig om bij het ontwerpen rekening te kunnen houden met de bestaande electriciteitskabels? 
* Wat zijn de maten en ligging van de electricitietskabels?
  *  Amsterdam werkt met een uitlegschema: per type kabel diameter, dekking (=diepte) en vrije werkruimte (=schrikruimte, minimale afstand tot andere objecten.) In IMKL wordt geen onderscheid gemaakt voor type kabels, transport, middenspanningskabel of huisaansluiting dus weet de ontwerper niet zeker of hij de juiste maten kent.
* Welke gegevens zijn bekend bij de beheerders van de electriciteitskabels?
* Welke informatiemodellen worden gebruikt door deze beheerders? IMBOR en/of IMKL?
* Dekken deze informatiemodellen de informatiebehoefte af?



## Use Case 2: ontwerpuitgangspunten nieuwe situatie

### Data 
#### Bomen
De ontwerper heeft de volgende input nodig vanuit normen, standaarden met ontwerparameters en eisen
* Welke parameters zijn nodig om te weten hoeveel ruimte de wortels van de boom nodig hebben?
* Is hier een datastandaard of informatiemodel voor?
* Dekt deze standaard de informatiebehoefte af?
* Welke andere eisen zijn er, om te garanderen dat de boom gezond blijft?
* Zijn er assets, waarbij een zekere afstand moet worden aangehouden tot de stam van de boom?
* Is hier een datastandaard of informatiemodel voor?
* Dekt deze standaard de informatiebehoefte af?
* Waar wijkt de huidige situatie af van die regels? 

#### Rioleringen
De ontwerper heeft de volgende input nodig vanuit normen, standaarden met ontwerparameters en eisen

* Welke parameters/eisen zijn nodig om te weten wat de afmetingen moeten zijn van de onderdelen van het riool en welke ligging het riool kan hebben? Welke diepte mag het riool hebben?
* Is hier een datastandaard of informatiemodel voor? GWSW?
* Dekt deze standaard de informatiebehoefte af?
* Zijn er assets, waarbij een zekere afstand moet worden aangehouden tot onderdelen van het riool?
* Is hier een datastandaard of informatiemodel voor?
* Dekt deze standaard de informatiebehoefte af?
* Waar wijkt de huidige situatie af van de ontwerpparameters? Leidt dit tot alternatieve "supotimale maar geaccepteerde afwijkingen van de eisen en parameters?"
* Je hebt voor bepaalde analyses van afwatering en je oppervlaktewaternetwerk ook BOR-gegevens nodig. Een oppervlaktewatersysteem bestaat ook uit Watergangen, Watervlaktes, Duikers etc. Het is vaak zo dat gemeentes en waterschappen de waterpeilen, oppervlaktes, bergende vermogens bepalen. Het bergende oppervlak en het bergende vermogen van verharding en gras- en kruidachtigen kan ook relevant zijn, evenals het type verharding (Betonverharding, Elementenverharding, Asfaltverharding). 




#### Electriciteitskabels
De ontwerper heeft de volgende input nodig vanuit normen, standaarden met ontwerparameters en eisen

* Welke parameters/eisen zijn nodig om te weten wat de afmetingen moeten zijn van de electriciteitskabels en welke ligging deze kunnen hebben? Welke diepte mag de kabel hebben?
* Is hier een datastandaard of informatiemodel voor? IMKL?
* Dekt deze standaard de informatiebehoefte af?
* Zijn er assets, waarbij een zekere afstand moet worden aangehouden tot electirciteitskabels?
* Is hier een datastandaard of informatiemodel voor?
* Dekt deze standaard de informatiebehoefte af?
* Waar wijkt de huidige situatie af van de ontwerpparameters? Leidt dit tot alternatieve "suboptimale maar geaccepteerde afwijkingen van de eisen en parameters?"

## Use Case 3: In kaart brengen beleid en plannen 

### Data 
#### Bomen
De ontwerper heeft de volgende input nodig vanuit beleidsdoelen en een strategisch assetmanagementplan:

* Is er een plankaart / toekomstvisie / groenplan bomenarchitectuur waarop aangegeven staat welke bestaande en nieuwe bomen in de toekomst aanwezig moeten zijn?
* Is er een datastandaard voor deze informatie?
* Dekt deze standaard de informatiebehoefte af?


#### Rioleringen
De ontwerper heeft de volgende input nodig vanuit beleidsdoelen en een strategisch assetmanagementplan:

* Is er een plankaart / toekomstvisie / strategisch plan  waarop aangegeven staat welke stromen in de toekomst moeten worden afgevoerd via de riolering? Alleen het afvalwater van huishoudens en bedrijven, of ook van hemelwater? Is berekend waar afvoer van hemelwater noodzakelijk blijft? Welke bergingscapaciteit gewenst is? 
* Zit deze informatie in het GWSW? Is hier een andere informatiestandaard voor?
* Dekt deze standaard de informatiebehoefte af?



#### Electriciteitskabels
De ontwerper heeft als doel een ruimtereservering te kunnen maken voor toekomstige kabels en leidingen. 
De ontwerper heeft de volgende input nodig vanuit beleidsdoelen en een strategisch assetmanagementplan:

* Is er een plankaart / toekomstvisie / strategisch plan waarop aangegeven staat welke toekomstige capaciteit gevraagd wordt per aansluiting? Is dit  afhankelijk van een scenario voor de energietransitie? 
* Zit deze informatie in IMKL? Is hier een andere informatiestandaard voor?
* Dekt deze standaard de informatiebehoefte af?


