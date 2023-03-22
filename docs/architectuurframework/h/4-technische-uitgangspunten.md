# Technische uitgangspunten

## Inleiding

Dit hoofdstuk beschrijft de technische uitgangspunten en eisen aan de informatiemodellen en andere datastandaarden die gebruikt worden in de boven- en ondergrondse openbare ruimte.

### Duurzame correcte mapping

Om data in samenhang te kunnen bevragen is het nodig dat verschillende standaarden/modellen op elkaar 'gemapt' worden. In dit specifieke geval gaat het om de IMBOR ontologie en de GWSW ontologie. Data over de ondergrond is namelijk geclassificeerd naar die twee ontologieën. En inhoudelijk vergelijking tussen de twee is relatief eenvoudig te maken. CROW en Rioned hebben dit ook reeds gedaan. Echter de methode hiervoor en de vastlegging hiervan is specifiek voor deze mapping. Hierdoor is het voor gebruikers en softwareleveranciers ondoenlijk om zich hier op te baseren.

Wat nog ontbreekt is een standaardaanpak voor ontologie matching (ook wel "mapping" of "linking" genoemd). Ontologie matching is belangrijk in de heterogene omgeving waarin ontologieën worden ontworpen, ontwikkeld en geacht worden te werken. Methodologisch is het de moeite waard om relaties tussen ontologieën uit te drukken omdat dit het volgende mogelijk maakt:

- Beheersbare ontologieën: Werken met kleine en zelfvoorzienende modulaire ontologieën, in plaats van monolithische ontologieën.
- Data transformatie: Het uitdrukken van de verbanden tussen twee versies van dezelfde ontologie (de delta) of tussen versies van andere ontologieën, en dus het bijwerken van gegevens van de ene ontologie naar de andere.
- Gezamenlijke basis gebruiken: Het terugplaatsen van een ontologie in de context van een toplevel ontologie, waardoor deze meer consensueel wordt met andere ontologieën van dat domein.
- Conjunctief gebruik: Door ontologieën samen te gebruiken in hetzelfde proces of dezelfde toepassing kunnen interdisciplinaire projecten beter op elkaar aansluiten.

De laatste reden is vrij dringend. Momenteel wordt dit vaak overgelaten aan de softwareleveranciers of modelleurs, terwijl ontologie- (of "standaard"-)beheerders hier meer aandacht aan zouden kunnen en moeten besteden. Zeker softwareleveranciers die ontologieën moeten gebruiken in hun software hebben te maken met meerdere, gedistribueerde en evoluerende ontologieën. Voor hen is duidelijkheid over hoe die in samenhang te gebruiken zeer belangrijk. Voorspelbaarheid over de structuur van de afstemming en de informatie over herkomst, auteurschap en versiebeheer van deze afstemming wordt beschouwd als een grote stimulans voor toepassing.

Binnen dit project hanteren (en ontwikkelen we tegelijkertijd) daarom de [Ontology whitepaper](https://docs.crow.nl/ontology-alignment/whitepaper/) van CROW.
