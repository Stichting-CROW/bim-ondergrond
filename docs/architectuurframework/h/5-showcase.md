# Showcase Wallengebied

## Inleiding
De CROW heeft een showcase gemaakt waarbij het potentieel van het koppelen van uiteenlopende datastandaarden binnen de ondergrondse infrastructuur aan de licht is gebracht. Deze showcase, gesitueerd in het historische Wallengebied van Amsterdam, maakt de synergie tussen gemeentelijke datasets en die van samenwerkingspartners tastbaar.

## Doelstelling
Het project had twee primaire doelstellingen: ten eerste het demonstreren van de haalbaarheid om data uit diverse bronnen te integreren en ten tweede het bewijzen dat dergelijke integratie substantiële meerwaarde biedt door verdiept inzicht te verschaffen. Het gekozen proefgebied voor deze demonstratie was het Wallengebied, waar data uit verschillende domeinen – zoals KLIC (kabels en leidingen), IMBOR (beheer openbare ruimte), GWSW (stedelijk water), en Liander (netbeheer) – samengebracht werden om een compleet beeld te vormen van het gebruik van de ondergrondse ruimte.

## Aanpak
De methodologie bestond uit verschillende fasen, beginnend met het verzamelen en selecteren van datasets, gevolgd door het harmoniseren van de betrokken ontologieën en het omzetten van datasets naar RDF formaat voor verbeterde interoperabiliteit. Vervolgens werd een schema vertaling uitgevoerd naar NEN2660-2 RDF, waarna een ontology-alignment werd gerealiseerd om de samenhang tussen verschillende datamodellen te versterken. Het project culmineerde in het beschikbaar stellen van de geïntegreerde datasets via SPARQL-Endpoints en het creëren van een datastory om de opgedane inzichten te illustreren.

<figure>
<img src="./h/media/stappenplanshowcase.png" alt="Een visualisatie van de aanpak van de showcase">
<figcaption>De technische stappen in de aanpak van de showcase</caption>
</figure> 

## Uitvoering
### Datasets en Ontologieën Verzamelen
De initiële stap omvatte het verzamelen van relevante datasets uit het Wallengebied, afkomstig van diverse bronnen. Deze datasets werden geselecteerd op basis van hun representativiteit voor het gebied en omvatten gegevens over infrastructuur zoals kabels, leidingen, en waterbeheer.

<figure>
<img src="./h/media/Screenshot 2023-10-13 155615.png" alt="Een screenshot van eenb GIS kaart met de representatieve dataset (het gebied en de lagen)">
<figcaption>Een screenshot van de representatieve dataset (het gebied en de lagen)</caption>
</figure> 

### Van Geodata naar NEN 2660-2
Een sleutelelement in het project was de conversie van GIS-formaten naar RDF, wat de flexibiliteit van de datasets aanzienlijk vergrootte. Door middel van opensource software<a href="#footnote-1">[1]</a> werd deze conversie gerealiseerd, wat de weg vrijmaakte voor een gestructureerde en samenhangende dataomgeving. 

<p id="footnote-1">[1] Redmer van CROW heeft hiervoor <a href="https://github.com/redmer/rdf-geopackage">opensource software</a> geschreven. Hiermee kan op een generieke manier een GeoPackage omgezet worden naar RDF. Met de genoemde software kan vanuit een GeoPackage zeer platte (generieke) linked data worden gegenereerd. Met een extra conversie kan de data dan weer aansluiten op de gebruikte standaarden.

### Ontology Alignment
Een innovatieve stap binnen het project was het uitlijnen van de verschillende ontologieën, een proces waarbij de relaties tussen diverse datamodellen werden gedefinieerd. Dit zorgde voor een uniforme interpretatie en integratie van de data.

## Datastory
Het projectresultaat werd gevat in een interactieve datastory. Deze datastory demonstreert de mogelijkheden van federatieve query's en biedt een rijke, interactieve ervaring die de meerwaarde van geïntegreerde datastandaarden illustreert.

## Resultaat en Toekomstvisie
Het project heeft aangetoond dat het combineren van datasets uit verschillende bronnen niet alleen mogelijk is, maar ook essentiële inzichten biedt die voorheen onbereikbaar waren. Dit initiatief vormt een belangrijke stap richting een meer geïntegreerde en toegankelijke data-infrastructuur voor stedelijke ontwikkeling en beheer.

URL: 		https://datasets.crow.nl/projecten/-/stories/Datastandaarden-in-samenhang 

De toegankelijkheid van de datastory is gegarandeerd tot 1 januari 2025, waarna deze in PDF-vorm beschikbaar blijft. Dit project markeert een belangrijk moment in het streven naar een coherente en gecombineerde benadering van datastandaarden, met potentieel verstrekkende implicaties voor stedelijk beheer en planning.

