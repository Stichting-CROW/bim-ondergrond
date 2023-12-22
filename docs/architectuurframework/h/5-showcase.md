# Showcase


## Inleiding
CROW heeft een showcase gemaakt voor het verbinden van datastandaarden in de ondergrond met datasets van gemeente Amsterdam en samenwerkpartners in het Wallengebied. 

## Doel showcase
Het doel van dit project was aantonen dat 1) het mogelijk is om data uit verschillende gedistribueerde bronnen te combineren en 2) aan te tonen dat dit meerwaarde / meer inzicht geeft. Om dit aan te tonen is besloten om binnen één gebied data te combineren uit verschillende ‘bronnen’. In dit geval was dit:
* KLIC data (bekend van de graafmeldingen; kabels en leidingen)
* IMBOR data (beheer openbare ruimte)
* GWSW data (stedelijk water)
* Liander data (netbeheerder)

Door deze bronnen te combineren zou er een nagenoeg volledig overzicht moeten kunnen ontstaan van het ondergronds ruimtegebruik. 


## Aanpak

Om het doel te realiseren zijn (hoog over) de volgende stappen ondernomen
<ol><li>Datasets verzameld (4 maal)</li>
<ul><li>Representatieve selectie gemaakt</li></ul>
<li>Betrokken ontologieën (datamodellen) verzameld (4 maal)
<li>Datasets omgezet naar RDF (3 maal)
<ul><li>“RDF-Geopackages” ontwikkeld</li></ul>
<li>RDF omgezet naar NEN2660-2 RDF
<ul><li>Schema vertaling gemaakt</li></ul>
<li>Ontology-alignment gemaakt 
<ul><li>Ontology-alignment-standaard ontwikkeld</li></ul>
<li>Verschillende RDF-sets beschikbaar gesteld als SPARQL-Endpoints
<li>Federatieve query’s gemaakt
<li>Datastory gemaakt</li></ol>

## Verzamelen datasets en ontologiën
Allereerst zijn er datasets verzameld. Dit betreft instantiedata van assets binnen het Wallengebied. Specialisten vanuit Amsterdam hebben data uit verschillende pakketten/bronnen geleverd, te weten IMBOR-data, GWSW-data, KLIC-data en Liander-data. Deze datasets hebben allemaal hun eigen datamodel (ontologie); deze modellen zijn ook verzameld. Vervolgens is een representatieve selectie gemaakt van assets binnen een selectief gebied. Dit is gedaan om het proces overzichtelijk te houden. 

Deze datasets zijn niet open beschikbaar. Wel is er een screenshot gemaakt om een idee te geven.

<figure>
<img src="./h/media/Screenshot 2023-10-13 155615.png" alt="Een screenshot van eenb GIS kaart met de representatieve dataset (het gebied en de lagen)">
<figcaption>Een screenshot van de representatieve dataset (het gebied en de lagen)</caption>
</figure> 

## Van Geodata naar NEN 2660-2
Behalve de GWSW-data, waren de gegevenssets niet beschikbaar in RDF, maar in verscheidene GIS-formaten. Om de data goed te combineren was een omzetting naar RDF (de techniek achter LinkedData) nodig. Redmer van CROW heeft hiervoor [opensource software](https://github.com/redmer/rdf-geopackage) geschreven<a href="#footnote-1">[1]</a>. Hiermee kan op een generieke manier een GeoPackage omgezet worden naar RDF. Met de genoemde software kan vanuit een GeoPackage zeer platte (generieke) linked data worden gegenereerd. Rijen uit featuretabellen worden geo:Features met arbitraire relaties en een geo:Geometry. Rijen uit niet-feature-tabellen worden geïnstantieerd met arbitraire eigenschappen.

Deze generieke RDF is omgezet naar de regels die gesteld worden volgens de NEN2660-2. Omdat RDF zo flexibel is, is meestal een ‘schema-definitie’ nodig om de data die in RDF staat eenvoudig leesbaar te maken. Hier wordt bijvoorbeeld gezegd waar precies in de RDF de geometrie van een feature gevonden kan worden. 

<p id="footnote-1">[1] Deze software is opensource ontwikkeld en gedistribueerd en wordt nu al gebruikt/bekeken door andere organisaties waaronder Geonovum (https://github.com/redmer/rdf-geopackage) 


## Ontology alignment
Het volgende innovatieve-onderdeel  van het project is het maken van een ontology-alignment. Hier wordt er vanuit gegaan dat de beheerders van de ontologieën (bijvoorbeeld CROW voor IMBOR en Rioned voor GWSW) definiëren hoe hun ontologieën zich tot elkaar verhouden. Door dit niet op een project of bij een bronhouder te doen, maar juist bij de partij die verstand heeft van het model hoeft dit maar één keer gedaan te worden. Er is/was echter geen standaard voor het maken, distribueren en het beheren van zo’n alignment. Daarom is [deze voorgesteld][whitepaper]<a href="#footnote-2">[2]</a> door CROW. Vervolgens is voor dit project een representatief voorbeeld-alignment gemaakt van IMBOR, GWSW, KLIC en Liander. 
* Door dit extra model worden bijvoorbeeld de relaties tussen GWSW en IMBOR klassen geformaliseerd, maar ook tussen GWSW en IMBOR eigenschappen
* Deze alignment is een eerste opzet, die wordt vanuit het IMBOR en GWSW project geformaliseerd.

<p id="footnote-2">[2] Dit whitepaper is ook opensource ontwikkeld en gedistribueerd en is inmiddels door meerdere partijen gereviewd. De hoop is hier een industrie standaard van te maken.

## Datastory maken
Om vervolgens het concept en de waarde hiervan aan te tonen zijn de verschillende RDF-sets geüpload naar een LinkedData-platform. Hierdoor kan de data nu middels een SPARQL-Endpoint aangeroepen worden. Er zijn federatieve query’s gemaakt (query’s die meerdere datasets tegelijkertijd bevragen) waarin verschillende usecases (aan)getoond worden. Deze zijn verwerkt in een datastory, met uitleg, interactieve tabellen en kaarten. 
Nu kunnen we dus federatieve vragen stellen als: ‘geef me alles in dit gebied met een aanlegjaar na 1950’. We creeren dus volledig overzicht over de ‘silo's’ heen.


De aanpak van de showcase wordt in onderstaande afbeelding gevisualiseerd. Met de kaders wordt de essentiële stap aangegeven die voor dit project van belang is: het structureren en laten samenhangen van standaarden.

<figure>
<img src="./h/media/stappenplanshowcase.png" alt="Een visualisatie van de aanpak van de showcase">
<figcaption>De aanpak van de showcase</caption>
</figure> 


## Resultaat
Het resultaat is moeilijk te omschrijven in woorden, vandaar dat dit geprobeerd is te vatten in een datastory. Deze story is online te raadplegen (zie bijlage) en vertelt het verhaal van wat er mogelijk is als data en datastandaarden in samenhang bevraagd kunnen worden

Logingegevens datastory: Datastandaarden in Samenhang 


URL: 		https://datasets.crow.nl/projecten/-/stories/Datastandaarden-in-samenhang 
Email address:	snuffelaccountcrow@rix.33mail.com
Password:	#####

Als je op de link klikt, krijg je eerst de mededeling dat er geen datastory te vinden is. Log je vervolgens in, dan zie je de datastory. Lees deze rustig door en zoom in-en uit en klik op de bijgevoegde kaarten voor ondersteuning van het verhaal.
Wat je kan doen in de datastory, het bevragen van de data, kan natuurlijk allemaal al lang in GIS. Het verschil is hier de onzichtbare werking van het publiceren van verschillende datasets op basis van verschillende, maar samenhangende datastandaarden. En het feit dat je dan, zonder de data nog verder te moeten inlezen, cureren en bewerken aan de slag kan gaan. 

<p class="note" title="Beschikbaarheid datastory">
Deze datastory blijft in de lucht tot 1 januari 2025. Daarna is deze alleen nog beschikbaar als <a href="/docs/architectuurframework/h/media/Datastandaarden in samenhang BIM in de ondergrond - CROW dataprojecten - dataset.crow.nl.pdf">pdf</a>.
</p>

[whitepaper]: https://docs.crow.nl/ontology-alignment/whitepaper/