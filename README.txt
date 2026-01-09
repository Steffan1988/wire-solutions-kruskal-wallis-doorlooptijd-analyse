# Doorlooptijdanalyse per Incidentcategorie – Wire Solutions

Deze repository bevat het Jupyter Notebook dat is gebruikt voor de
statistische analyse van doorlooptijden van incidenten binnen de
servicedesk van Wire Solutions. De analyse is uitgevoerd als onderdeel
van het afstudeeronderzoek en dient als kwantitatieve verdieping van
**Deelvraag 2: Doorlooptijden en behandelgroepen**.

De focus ligt op het vaststellen of de doorlooptijd van incidenten
significant verschilt tussen incidentcategorieën, en of deze verschillen
inhoudelijk relevant zijn voor SLA-afspraken en capaciteitsinrichting.

---

## Doel van de analyse

Het doel van deze analyse is om inzicht te krijgen in:

- verschillen in doorlooptijd tussen incidentcategorieën;
- de mate waarin deze verschillen statistisch significant zijn;
- de omvang en relevantie van deze verschillen (effectgrootte);
- de spreiding en uitschieters per categorie.

De analyse is bedoeld ter statistische onderbouwing van bevindingen in
het onderzoeksrapport en vormt geen operationeel voorspellings- of
monitoringsmodel.

---

## Inhoud van het notebook

Het notebook bevat onder andere:

- inladen en opschonen van incidentdata;
- verwijderen van dubbele registraties op basis van incidentnummer;
- selectie en validatie van doorlooptijden;
- toepassing van de Kruskal–Wallis-toets;
- berekening van de effectgrootte (epsilon squared);
- visualisatie van doorlooptijden per incidentcategorie met boxplots
  (inclusief logaritmische schaal).

De volgorde van incidentcategorieën in de visualisaties is afgestemd
op de structuur en terminologie van het onderzoeksrapport.

---

## Dataset

De gebruikte dataset is geanonimiseerd en niet opgenomen in deze
repository in verband met vertrouwelijkheid. De dataset bevat per
incident minimaal de volgende velden:

- incident nummer;
- incidentcategorie;
- totale minuten open;
- prioriteit incident.

Voor de analyse is gewerkt met één unieke registratie per incident.
Incidenten met ontbrekende of niet-logische doorlooptijden zijn
uitgesloten.

---

## Interpretatie en context

De resultaten van dit notebook worden gebruikt als statistische
onderbouwing van de analyse in het onderzoeksrapport. De uitkomsten
laten zien dat doorlooptijden significant verschillen tussen
incidentcategorieën en dat deze verschillen ook inhoudelijk relevant
zijn.

De analyse ondersteunt de conclusie dat één uniforme SLA voor alle
incidenten niet realistisch is en dat oplostijden sterk samenhangen
met complexiteit en escalatieniveau.

De conclusies uit dit notebook dienen ter interpretatie en reflectie
en zijn niet bedoeld als direct sturingsinstrument.

---

## Technische omgeving

De analyse is uitgevoerd met Python en gangbare data-analysebibliotheken,
waaronder:

- pandas  
- numpy  
- matplotlib  
- scipy  

Het notebook is reproduceerbaar met een dataset die dezelfde structuur
en kolomnamen hanteert.

---

### Opmerking

Dit notebook vormt een **aanvullende statistische analyse** binnen het
afstudeeronderzoek en dient in samenhang met het onderzoeksrapport
te worden geïnterpreteerd.
