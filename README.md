# Doorlooptijdanalyse per Incidentcategorie – Wire Solutions

Deze repository bevat een Jupyter Notebook met een analyse van de
doorlooptijd van incidenten binnen de servicedesk van Wire Solutions.
De analyse is uitgevoerd als onderdeel van het afstudeeronderzoek en
ondersteunt **Deelvraag 2: Doorlooptijden en behandelgroepen**.

De focus ligt op het vergelijken van doorlooptijden tussen
incidentcategorieën en het bepalen of deze verschillen statistisch
significant en relevant zijn voor SLA-afspraken.

---

## Doel van de analyse

Het doel van deze analyse is om inzicht te krijgen in:

- verschillen in doorlooptijd tussen incidentcategorieën;
- de statistische significantie van deze verschillen;
- de omvang en spreiding van doorlooptijden per categorie.

De analyse dient als onderbouwing van het onderzoeksrapport en is niet
bedoeld als operationeel voorspellingsmodel.

---

## Inhoud van het notebook

Het notebook bevat onder andere:

- opschonen en dedupliceren van incidentdata;
- selectie van geldige doorlooptijden;
- toepassing van de Kruskal–Wallis-toets;
- berekening van de effectgrootte (epsilon squared);
- visualisatie van doorlooptijden met boxplots (incl. log-schaal).

De volgorde van categorieën in de grafieken sluit aan bij het
onderzoeksrapport.

---

## Dataset

De gebruikte dataset is geanonimiseerd en daarom niet opgenomen in deze
repository. Per incident zijn minimaal de volgende velden gebruikt:

- incident nummer;
- incidentcategorie;
- totale minuten open.

Elke waarneming vertegenwoordigt één uniek incident.

---

## Interpretatie en context

De resultaten laten zien dat doorlooptijden significant verschillen
tussen incidentcategorieën en dat deze verschillen ook inhoudelijk
relevant zijn. Dit ondersteunt de conclusie dat één uniforme SLA niet
passend is voor alle typen incidenten.

De analyse is bedoeld ter interpretatie en reflectie en niet als direct
sturingsinstrument.

---

## Technische omgeving

De analyse is uitgevoerd met Python en de volgende libraries:

- pandas  
- numpy  
- matplotlib  
- scipy  

Het notebook is reproduceerbaar met een dataset met dezelfde structuur.

---

### Opmerking

Dit notebook vormt een **aanvullende analyse** binnen het
afstudeeronderzoek en dient in samenhang met het onderzoeksrapport te
worden gelezen.

