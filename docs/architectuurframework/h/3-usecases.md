# Use Cases

<dfn data-lt="Use case">Use case</dfn>
<dd>Beschrijving van een systeem vanuit het gebruikersperspectief, met een actor, de initiator van de interactie, en het systeem zelf als een opeenvolging van eenvoudige stappen. […] Actoren kunnen eindgebruikers, andere systemen of hardware (apparatuur) zijn. Elke usecase is een complete serie van zogenaamde "events", beschreven vanuit het standpunt van de actor. Bron: <a href="https://nl.wikipedia.org/wiki/Usecase">Wikipedia</a></dd>

<figure>
<img src="./h/media/werkwijzeusecases.png" alt="Visualisatie hoe vanuit een use case met werkproces, informatiebehoefte en gebruikte systemen gewerkt kan worden aan het afspreken van datapakketjes die worden uitgewisseld tussen landelijke vorozieningen, in de beheerorganisaties, in de projectorganisaties en met opdrachtnemers in het stedelijke gebied">
<figcaption>De opgave voor partijen die werken in het stedelijke gebied: Van use case naar begrijpelijke datapakketjes</caption>
</figure>


## Use case 1 

Use Case 1: In samenhang bevragen van data om het ondergrondse ruimtegebruik in kaart te brengen

## Actoren

### Gebruikers

* Databeheerders
* Planners binnen een integraal project van de gemeente

### Data

* Rioleringsgegevens gestructureerd volgens GWSW (uit specialistisch pakket, of ook uit Gisib?)
* BOR gegevens gestructureerd volgens IMBR (uit Gisib?)

## Doelstelling

Het combineren van de gegevens gestructureerd via GWSW, met gegevens gestructureerd via het IMBOR om een zo volledige mogelijk beeld van het ondergrondse ruimtegebruik te krijgen.

## Beschrijving

* Uit het Rioleringsysteem moeten type, liggings- en dimensiegegevens komen van een representatief aantal objecten;
* Uit het BORsysteem moeten type, liggings- en dimensiegegevens komen van een representatief aantal objecten;
* Beiden zijn als RDF beschikbaar en geclassificeerd aan respectievelijk GWSW en IMBOR;
* Middels de alignment die gemaakt is worden conclusies getrokken over welke objecten hetzelfde zijn en zodoende welke gegevens gecombineerd kunnen worden;
* Deze 'nieuwe' gegevenset wordt beschikbaar gemaakt in een (visueel) systeem;
* De gebruiker gebruikt de gecombineerde gegevens om het ondergrondse ruimtegebruik in kaart te hebben.

## Alternatieve scenario's

* Als de gegevens niet correct worden gecombineerd, kan het zijn dat het volledige ondergrondse ruimtegebruik niet correct wordt weergegeven. In dat geval moet de gebruiker de gegevens opnieuw combineren of de fout corrigeren.
* Als er wijzigingen worden aangebracht in de beiden datsets, moeten de gegevens opnieuw worden geëxporteerd en gecombineerd om het volledige ondergrondse ruimtegebruik up-to-date te houden.

## Vragen aan experts

Om een representatieve dataset te kunnen behandelen staan er nog enkele vragen op m.b.t. deze use case:

<ul>
<li>Om welke systemen gaat het precies?
<li>Welke Objecttypen gaat het om (e.g. Leiding, Put, Boom, Kabel, Lichtmast, Ondergrondse container, ...)?
<ul><li>Wat is een (selectieve) subset hiervan om het idee goed aan te kunnen tonen?</li></ul>
<li>Is hier dan ook data voor beschikbaar (in het Wallengebied)?
<ul><li>Is deze dan ook als RDF beschikbaar?
<li>Zijn deze dan ook geclassificeerd naar GWSW en IMBOR</li></ul>
<li> Welk systeem zou gebruikt kunnen worden voor de gecombineerde weergave? </li></ul>

# Achtergrond informatie

## Hoog over scenario's

* Uitwisseling tussen twee systemen die de integratie van rioleringsgegevens vereist in een BOR-systeem (het ene systeem is conform IMBOR ingedeeld, het andere systeem conform een interpretatie van de GWSW-ontologie)
* Uitwisseling tussen twee systemen die de integratie van BOR-gegevens vereist in een rioleringssysteem (bijv. verhardingen, wadi's, meubilair) (het ene systeem is conform IMBOR ingedeeld, het andere systeem conform een interpretatie van de GWSW-ontologie)
* GWSW-dataset uitwisselen vanuit een integraal beheersysteem dat conform IMBOR is ingedeeld (bijv. hoe kom je van IMBOR naar .orox)
* IMBOR als standaard gebruiken voor vaste objectgegevens, maar daar GWSW-dynamische gegevens bij willen registreren
* Gegevens van aannemer die volgens GWSW kan inspecteren/etc. opnemen in beheersysteem conform IMBOR

In een gemeente kan het best zo zijn dat Assetmanager Riolering een applicatie voor Riolering gebruikt en andere Assetmanagers een integraal systeem. Die eerste Assetmanager moet dan ofwel data aan de anderen leveren voor het integrale beeld (situatie 1); ofwel data ontvangen van de anderen voor het verkrijgen van overzicht/bepaalde berekeningen (situatie 2)

## Use case alternatief 1

Je hebt voor bepaalde analyses van afwatering en je oppervlaktewaternetwerk ook BOR-gegevens nodig. Een oppervlaktewatersysteem bestaat ook uit Watergangen, Watervlaktes, Duikers etc. Het is vaak zo dat gemeentes en waterschappen de waterpeilen, oppervlaktes, bergende vermogens bepalen. Het bergende oppervlak en het bergende vermogen van verharding en gras- en kruidachtigen kan ook relevant zijn, evenals het type verharding (Betonverharding, Elementenverharding, Asfaltverharding). Ik weet dat Assetmanagers riolering die info gebruiken om de volgende dingen te bepalen (de exacte rekensommen ken ik niet):

1. Wat is het afgekoppelde oppervlak?
2. Zijn de afwateringsvoorzieningen voldoende voor dit verharde gebied?
3. Wat is de doorstroming van het oppervlaktewatersysteem?
4. Wat is de bergingscapaciteit van het oppervlaktewatersysteem?
5. Wat voor objecten liggen er boven de uit te graven/te vervangen riolering?
6. E.d. vragen

