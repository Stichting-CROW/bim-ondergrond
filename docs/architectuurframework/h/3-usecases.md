# Use Cases 

## Definitie use case

<dfn data-lt="Use case">Use case</dfn>
<dd>Beschrijving van een systeem vanuit het gebruikersperspectief, met een actor, de initiator van de interactie, en het systeem zelf als een opeenvolging van eenvoudige stappen. […] Actoren kunnen eindgebruikers, andere systemen of hardware (apparatuur) zijn. Elke usecase is een complete serie van zogenaamde "events", beschreven vanuit het standpunt van de actor. Bron: <a href="https://nl.wikipedia.org/wiki/Usecase">Wikipedia</a></dd>

<figure>
<img src="./h/media/werkwijzeusecases.png" alt="Visualisatie hoe vanuit een use case met werkproces, informatiebehoefte en gebruikte systemen gewerkt kan worden aan het afspreken van datapakketjes die worden uitgewisseld tussen landelijke voorzieningen, in de beheerorganisaties, in de projectorganisaties en met opdrachtnemers in het stedelijke gebied">
<figcaption>De opgave voor partijen die werken in het stedelijke gebied: Van use case naar begrijpelijke datapakketjes</caption>
</figure>

## Use cases bij het ontwerpen

De scope van de use cases zijn de use cases die binnen het ontwerpproces vallen. In het voorbeeld waar mee gewerkt wordt op basis van de casus Wallengebied zijn dit de volgende use cases:
1. De ontwerper wil de bestaande ligging van ondergrondse objecten en relevante bovengrondse objecten in kaart brengen;
2. De ontwerper wil weten wat de eisen en parameters zijn bij het ontwerpen van een nieuwe situatie;
3. De ontwerper wil weten welke ondergronds objecten aanwezig moeten zijn in de nieuwe situatie: input vanuit beleid en de planfase. 
4. De ontwerper wil principeprofielen maken voor de inrichting van de ondergrond van een straat met aan één zijde gebouwen en aan de andere zijde een gracht en daarbij de afwegingen weergeven bij het ontwerp, zoals afwijking van de eisen over afstanden tot andere objecten omdat er niet voldoende ruimte is.
5. De ontwerper wil aangeven welke variabelen leiden tot welk principeprofiel, zodat er een onderbouwde afweging gemaakt kan worden voor het te kiezen principeprofiel bij elke straat.


## Use case 1: in kaart brengen bestaande situatie 

Use Case 1: In samenhang bevragen van data om het bestaande ondergrondse ruimtegebruik in kaart te brengen.

## Doelstelling

Het combineren van de gegevens gestructureerd via GWSW/IMBOR/IMKL/IMGeo, om een zo volledige mogelijk beeld van het ondergrondse ruimtegebruik te krijgen.

## Actoren

### Gebruikers

* Databeheerders
* Ontwerpers binnen een integraal project van een gemeente

## Beschrijving

### Stap 1: Verzamelen datasets
De ontwerper verzoekt de beheerders van de assets om de datasets die nodig zijn voor het in kaart brengen van de bestaande situatie aan te leveren. Deze datasets zijn gebaseerd op de open standaarden IMBOR, IMKL, IMGeo en GWSW (en meer?)

* Uit het Rioleringsysteem moeten type, liggings- en dimensiegegevens komen van een representatief aantal objecten;
* Uit het BORsysteem moeten type, liggings- en dimensiegegevens komen van een representatief aantal objecten;
* Uit NTB systemen ....
* Alle datasets zijn als RDF beschikbaar en geclassificeerd aan respectievelijk GWSW en IMBOR en andere standaarden.


### Stap 2: Verwerken datasets
De ontwerper verwerkt de aangeleverde datasets in het ontwerpproces. Hierbij worden de datasets geanalyseerd en omgezet naar een bruikbaar format.
* Middels de alignment die gemaakt is tussen standaarden worden conclusies getrokken over welke objecten hetzelfde zijn en zodoende welke gegevens gecombineerd kunnen worden;
* Deze 'nieuwe' gegevenset wordt beschikbaar gemaakt in een (visueel) systeem;
* De gebruiker gebruikt de gecombineerde gegevens om het ondergrondse ruimtegebruik in kaart te hebben.

### Stap 3: Onderzoeken compleetheid en informatie
Voordat de ontwerper aan de slag gaat met de verwerkte datasets, wordt onderzocht of de datasets compleet zijn en voldoende informatie bevatten om mee te kunnen werken.

### Stap 4: In kaart brengen bestaande situatie
Met behulp van de verwerkte datasets en eventueel aangevuld met eigen metingen, brengt de ontwerper de bestaande situatie in kaart.

## Alternatieve scenario's

* Als de gegevens niet correct worden gecombineerd, kan het zijn dat het volledige ondergrondse ruimtegebruik niet correct wordt weergegeven. In dat geval moet de gebruiker de gegevens opnieuw combineren of de fout corrigeren.
* Als er wijzigingen worden aangebracht in de beiden datsets, moeten de gegevens opnieuw worden geëxporteerd en gecombineerd om het volledige ondergrondse ruimtegebruik up-to-date te houden.


## Data 
#### Bomen
<div class="issue" data-number="10"></div>

#### Rioleringen
<div class="issue" data-number="11"></div>

* Rioleringsgegevens gestructureerd volgens GWSW (uit specialistisch pakket, of ook uit Gisib?)

#### Gas

#### Drinkwater

#### Electriciteitskabels
<div class="issue" data-number="12"></div>

#### Warmtenet

#### Hemelwaterafvoer

#### Overige relevante objecten
* BOR gegevens gestructureerd volgens IMBOR (uit Gisib?)?













# Achtergrond informatie

## Hoog over scenario's

* Uitwisseling tussen twee systemen die de integratie van rioleringsgegevens vereist in een BOR-systeem (het ene systeem is conform IMBOR ingedeeld, het andere systeem conform een interpretatie van de GWSW-ontologie)
* Uitwisseling tussen twee systemen die de integratie van BOR-gegevens vereist in een rioleringssysteem (bijv. verhardingen, wadi's, meubilair) (het ene systeem is conform IMBOR ingedeeld, het andere systeem conform een interpretatie van de GWSW-ontologie)
* GWSW-dataset uitwisselen vanuit een integraal beheersysteem dat conform IMBOR is ingedeeld (bijv. hoe kom je van IMBOR naar .orox)
* IMBOR als standaard gebruiken voor vaste objectgegevens, maar daar GWSW-dynamische gegevens bij willen registreren
* Gegevens van aannemer die volgens GWSW kan inspecteren/etc. opnemen in beheersysteem conform IMBOR

In een gemeente kan het best zo zijn dat Assetmanager Riolering een applicatie voor Riolering gebruikt en andere Assetmanagers een integraal systeem. Die eerste Assetmanager moet dan ofwel data aan de anderen leveren voor het integrale beeld (situatie 1); ofwel data ontvangen van de anderen voor het verkrijgen van overzicht/bepaalde berekeningen (situatie 2)
