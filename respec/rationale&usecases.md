# Rationale en use cases
## Rationale
Taxonimieën en thesauri zijn al eeuwen oud en vinden hun oorsprong in het toegankelijk maken, c.q. toegankelijk van teksten op papyrusrollen en later op perkament en papier. Waar thesauri in het verleden werden ontworpen voor informatieprofessionals die zijn opgeleid in indexeren en zoeken, is er tegenwoordig vooral vraag naar vocabulaires die ongetrainde gebruikers helpen bij het intuïtief vinden van informatie en naar vocabulaires die redeneren door machines mogelijk maken. De ISO 25964 standaard voor thesauri maakt zoals ze zelf in de inleiding aangeeft de transitie die nodig is om compatibel te zijn met de digitale wereld van informatiemanagement. Daarbij gaat het om het zoeken en vinden van informatie in digitale registraties. 

De gedachte achter zo'n index is dat de informatiezoeker via een term, gerelateerde termen, alternatieve termen of meer of minder preciese termen de data vindt bij het concept dat met die term wordt aangeduid. 
* Wikipedia definieert een concept (Latijn concipere - conceptum: bijeen-nemen, be-grijpen, be-vatten) als een cognitieve (mentale) eenheid, waarin meerdere ideeën, op grond van hun cognitief ervaren verwantschap, worden samengevat tot een hogere cognitieve klasse. Een begrip is een synoniem van een concept.
  * Dit betekent in de eerste plaats dat een concept iets is dat in de hoofden van mensen zit en verwijst naar iets in de fysieke werkelijkheid. Een concept is dus niet de fysieke werkelijkheid, maar verwijst daarnaar. In de context van documenten en (digitale) registraties gaat het per definitie om een gedeelde werkelijkheid. En in de context van de overheid in een rechtstaat om een gedeelde juridische werkelijkheid. 
  * In de tweede plaats is een concept als 'eenheid van denken' iets essentieel anders als een dataklasse of dataobject dat in de informatiekunde wordt gebruikt als verwijzing naar een object ('iets') in de fysieke wereld waarover data worden vastgelegd of naar een eigenschap van zo'n object. Een concept is typisch talig en primair bedoeld voor mensen, hoewel de ISO 25964 ook het redeneren door machines expliciet benoemt en  semantic AI steeds meer mogelijkheden biedt.
* Er ligt ook ergens een knip tussen een samenhangende beschrijving van concepten in een thesaurus en een model van klassen in een ontologie. Wikipedia definieert een ontologie (van het Grieks ὀν = zijnde en λόγος = woord, leer) of zijnsleer als de filosofische tak die het wezen onderzoekt dat achter de waargenomen werkelijkheid schuilgaat. De ontologie onderzoekt en beschrijft de eigenschappen, of breder: het zijn van het geheel van dingen, entiteiten of zijnden waarvan aangenomen wordt dat ze bestaan of beter: zijn. De ontologie gaat dus over de dingen zelf, hun 'zijn', terwijl concepten gaat over de 'gedachte'. In de praktijk is het wel handig als deze twee op elkaar aansluiten. In de psychiatrie zijn voldoende voorbeelden waar de 'gedachte' over de wereld niet matcht met de wereld zelf.
  * In de praktijk is een ontologie de basis voor een datamodel. Ook hier geldt dat een datamodel waarin de structuur van dingen en de data die daarover worden vastgelegd goed moet aansluiten bij de betreffende dingen in de fysieke wereld (zoals beschreven in de ontologie) en de eigenschappen van die dingen.
  * Soms wordt een ontologie ook gezien als een nog wat gedetailleerdere conceptualisering dan een thesaurus. Dit gebeurt bijvoorbeeld in de NEN 2660. In dit profiel doen we geen uitspraak over 

Uit een inventarisatie binnen de werkgroep kwamen 4 uses cases naar voren, die overeenkomen met verschillende niveaus van diepgang waarop een begrippenkader kan worden beschreven: 
- Begrippenlijst. Dit is de meest eenvoudige use case, die voor Geonovum geldt. In het geo domein is het vaak voldoende om de dingen die op de kaart moeten komen als begrip te definiëren, zonder verdere onderlinge relaties tussen de begrippen te definiëren.
- Taxonomie: Hiërarchische relaties zijn soms ook relevant voor Geonovum. Zo kan een kaart wegen, en terrein bevatten, waarbij een weg een autoweg, spoorweg of vaarweg kan zijn, een terrein een bos, stad, weiland etc. kan zijn.
- Thesaurus: Voor veel begrippencatalogi zijn ook de relaties tussen begrippen relevant. Dit geldt voor het Kadaster, DUO en de stelselcatalogus voor de basisregistraties. Zo is een zakelijk recht bij het Kadaster een recht (hiërarchische relatie) op een onroerende zaak (relatie met een ander begrip). De stelselcatalogus voor de basisregistraties wil ook concepten van verschillende registraties met elkaar verbinden, bijvoorbeeld een persoon (in de BRP) die gerelateerd kan zijn aan een organisatie (in het HR).
- Een voorbeeld van extra semantiek is het domein van rechtshandelingen, wat bijvoorbeeld bij het Kadaster relevant is. Een verkoper (actor) levert (rechtshandeling) een onroerende zaak (object) aan een koper (actor), welke overeenkomst bij akte wordt vastgelegd door een notaris (agent). Door dit soort semantiek toe te voegen wordt nog beter zichtbaar hoe begrippen samenhangen in een bepaalde context.

Het profiel modulair opgebouwd. Met de basale bouwstenen kan laagdrempelig een eenvoudige begrippenlijst worden gepubliceerd. Door nieuwe bouwstenen toe te voegen kan steeds meer semantiek aan een begrippenkader worden toegevoegd zodat een taxonomie, een thesaurus ontstaat of zelfs een thesaurus inclusief annotatie van voor rechtshandelingen relevante begrippen ontstaat.

Met metadata kan ook de geldigheid en zichtbaarheid (publicatiedatum) van een bepaalde versie van een begrip worden toegevoegd.

### Usecases

**User story DUO 1**  Transparantie.  Als wettelijk registerhouder wil ik dat ontwikkelaars, ondersteuners en gebruikers met een druk op de knop een passende en blijvende uitleg (de betekenis) van door mij verstrekte gegevens kunnen vinden, zodat zij deze juist kunnen interpreteren, hergebruiken en feedback kunnen geven.


**Usecase Geonovum 1** enkelvoudig beheer meervoudig gebruik (Must Have):
Als beheerder van informatiemodellen wil ik de begrippen van die informatie modellen eenmalig in linked-data beheren en door meerdere views (stelselcatalogus logius, conceptenbibliotheek geonovum etc…) ontsluiten. Enkelvoudig beheer meervoudig gebruik. Zodat ik met minimale inspanning maximaal profijt heb van de linked-data die ik beheer.
Daarvoor is het van belang dat het meta-model van mijn linked-data store interoperabel is met de linked data “front-ends” van andere linked-data catalogi.
**User story DUO 3**  Portabel. Als modellenautoriteit van een uitvoeringsorganisatie wil ik een (inter)nationaal koppelvlak waar ik begrippen inkomend en uitgaand kan ontsluiten zodat ik toekomstvast ben en onafhankelijk ben van tools en methoden [GGR: niet helemaal in lijn met Geonovum 1].

**User story DUO 2**  Interoperabel.  Als uitvoeringsorganisatie wil is dat wettelijke registers die ik nodig heb, hun begrippen volgens nationaal afgesproken naamgevings- en ontwerpregels opstellen zodat ik deze met een minimum aan inspanning kan inpassen in mijn eigen gegevensverwerking.
**Usecase geonovum 2** federatief zoeken(should have):
Ik wil graag linked data stores van anderen kunnen doorzoeken zodat ik vanuit de geonovum view op deze linked data (conceptenbibliotheek) vergelijkingen kan maken tussen begrippen uit verschillende catalogi

**Usecase geonovum 3** harmonisatie/disambiguatie(could have):
Ik wil graag relaties kunnen leggen tussen begrippen in verschillende catalogi. De belangrijkste doelen zijn daarbij harmonisatie (aangeven welke begrippen erg op elkaar lijken en kandidaat zijn voor harmonisatie) Disambigueren (begrippen die in eerste instantie op elkaar lijken maar toch op essentiële punten verschillen expliciet als niet hetzelfde aanmerken).

**Usecase geonovum 4** Begrippen kennen (versie) historie(should have):
Het is mogelijk naar een specifieke versie van een begrip te verwijzen of om naar de meest recente versie van een begrip te verwijzen. Dit is mogelijk met een eenduidige URI strategie.

**Usecase geonovum 5** Het is mogelijk de status van een begrip uit te drukken(could have):
Begrippen kunnen in ontwikkeling zijn, ze kunnen vastgesteld en geldig zijn of ze kunnen deprecated zijn, dus tussen bepaalde data waren ze geldig maar na een vastgelegde einddatum niet meer.