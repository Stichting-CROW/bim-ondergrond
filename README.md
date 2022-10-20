# Specificatie

Dit is de GitHub-repository voor het project waarmee CROW in opdracht van de CityDeal Openbare Ruimte in kaart brengt hoe data standaarden in samenhang te gebruiken om de ondergrond goed in beeld te brengen. 

Met alle maatschappelijke opgaven als energietransitie, klimaat adaptatie, diverse vervangingsopgaven (bestaande ondergrondse netwerken, kademuren, riolering etc) en het streven naar een gezonde en leefbare stad met een goede bodem en (grond)waterkwaliteit, is het steeds meer een puzzel om in de ondergrond alles passend te krijgen. We zullen hierbij meer integraal moeten werken. Hiervoor is goede informatie nodig over de functies en het ruimtegebruik in de ondergrond.
De informatie over de ondergrond wordt geproduceerd en beheerd door verschillende partijen.  Het zou een doorbraak zijn als verschillende tools op ieder moment de beschikbare informatie over de ondergrond zouden kunnen raadplegen en ontsluiten. Met daarbij als uitgangspunt dat data-eigenaren controle houden over hun eigen data en in hun eigen bedrijfsomgeving kunnen blijven werken.

Lees mee met het [Architectuur Framework](https://docs.crow.nl/bim-ondergrond/architectuurframework/) in ontwikkeling.

## Instructies voor redacteurs

1. **Werkversies**

   Werkversies worden continu gepubliceerd op `https://docs.crow.nl/bim-ondergrond/framework (logboek op [auto-publish]).

2. **Referentieversies**

   Bijvoorbeeld voor een review of consultatie; klik op [**Publiceer een bepaalde versie**](lifecycle) en vervolgens _Run workflow_.

3. **Een nieuw document toevoegen**

   Bijvoorbeeld voor een conceptueel model, API-beschrijving of uitwisselingsformaat; klik op [**Voeg een nieuw document toe**](add-doc) en kies _Run workflow_.

4. **Publicatie op crow.nl**

   Voor op de startpagina van _docs.crow.nl_: zie de [README van docs.crow.nl][publiceer-readme].
   Voor op crow.nl of de kennisbank: mail.

5. **Werken met ReSpec**

   ReSpec biedt structuur en presentatiemogelijkheden voor technische specificaties.
   Zoals informatiemodellen, uitwisselingsstandaarden en API-documentatie.

   ReSpec gebruikt [GfM](https://github.github.com/gfm/) als Markdown-specificatie.
   Lees ter referentie de [CROW-ReSpec-wiki] en de algemene [ReSpec-handleiding].

6. **Werken met Git en GitHub**

   Er zijn talloze handleidingen voor Git en GitHub.

   De webinterface van VS Code (druk op GitHub.com op <kbd>.</kbd>) of
   Visual Studio Code geïnstalleerd op je computer.
   Voor VS Code worden er ook aanbevolen extensies meegegeven in deze repository.

7. **Bijlagen, zoals afbeeldingen**

   Gebruik SVG-bestanden, bijvoorbeeld bewerkt met [draw.io](https://app.diagrams.net/).

[add-doc]: actions/workflows/add-doc.yaml
[auto-publish]: actions/workflows/auto-publish.yaml
[lifecycle]: actions/workflows/lifecycle.yaml
[publiceer-readme]: https://github.com/stichting-crow/stichting-crow.github.io/blob/main/README.md#publiceren
[crow-respec-wiki]: https://github.com/stichting-crow/respec/wiki
[respec-handleiding]: https://respec.org/docs/
