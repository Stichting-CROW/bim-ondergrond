# Showcase


## Inleiding
CROW heeft een showcase gemaakt voor het verbinden van datastandaarden in de ondergrond met datasets van gemeente Amsterdam en samenwerkpartners. Uitgevoerde activiteiten:

* Datasets vanuit GIS transformeren naar linked data
* Relaties leggen tussen de gebruikte informatiemodellen 
* Laten zien dat je door deze relaties queries kan uitvoeren over meerdere datasets.

Daarmee wordt aangetoond hoe handig het is, als datasets in linked data staan en de onderliggende informatiemodellen met elkaar verbonden zijn. 

## Samenstellen representatieve dataset

Als eerste zijn de aangeleverde bronbestanden omgezet naar een representatieve dataset:

* Hiervoor zijn alle aangeleverde bronsets in één Geopackage gezet
* Daarvan is doormiddel van een uitsnede een representatieve dataset gemaakt.

Deze datasets zijn niet open beschikbaar. Wel is er een screenshot gemaakt om een idee te geven.

<figure>
<img src="./h/media/Screenshot 2023-10-13 155615.png" alt="Een screenshot van eenb GIS kaart met de representatieve dataset (het gebied en de lagen)">
<figcaption>Een screenshot van de representatieve dataset (het gebied en de lagen)</caption>
</figure> 

## Geopackage naar rdf
Met behulp van [deze open source software](https://github.com/redmer/rdf-geopackage) zijn de Geopackages op een standaard manier omgezet naar RDF waar je vervolgens in kan zoeken met behulp van SPARQL-queries. 


Met de genoemde software kan vanuit een GeoPackage zeer platte (generieke) linked data worden gegenereerd. Rijen uit featuretabellen worden geo:Features met arbitraire relaties en een geo:Geometry. Rijen uit niet-feature-tabellen worden geïnstantieerd met arbitraire eigenschappen.

## Cureren van de dataset
Op de RDF zijn SPARQL-queries geschreven die de set omzet naar een ‘gecureerde’ graaf. Ofwel het handmatig verrijken van features en properites:
* Met IMBOR en GWSW classificaties 
* Met NEN2660-2 als ontologie 


## Alignment tussen standaarden

Vervolgens is ten behoeve van dit project een [proef-'alignment’](https://github.com/Stichting-CROW/bim-ondergrond/blob/main/code/alignment.ttl) gemaakt tussen de standaarden
* Door dit extra model worden bijvoorbeeld de relaties tussen GWSW en IMBOR klassen geformaliseerd, maar ook tussen GWSW en IMBOR eigenschappen
* Deze alignment is een eerste opzet, die wordt vanuit het IMBOR en GWSW project geformaliseerd.



## Resultaat
Bovenstaande hebben we allemaal werkend, maar het moet nog ‘geschaald’ worden. Ofwel we hebben het nu voor een paar objecttypen en eigenschappen gedaan om te zien of het werkt, maar we willen dit nog voor de hele representatie dataset doen. Dat is daarmee ook de volgende stap. 
Na die stap kunnen we dus federatieve vragen stellen als: ‘geef me alles in dit gebied met een aanlegjaar na 1950’. We creeren dus volledig overzicht over de ‘silo's’ heen.


