---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Python via .NET API-referentie"
description: 
type: docs
weight: 350
url: /nl/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Definieert de criteria waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP‑weergave.

Het type FilterCriteria bevat de volgende leden:
## Constructors
| Naam | Beschrijving |
| :- | :- |
| FilterCriteria() | Initialiseert een nieuw exemplaar van de klasse FilterCriteria |
## Eigenschappen
| Naam | Beschrijving |
| :- | :- |
| operation | Haalt op of stelt het criterium in dat is vastgesteld met FieldName, Test en Value en dat betrekking heeft op andere criteria in het filter. |
| field | Haalt op of stelt een [field](/tasks/python-net/aspose.tasks/filtercriteria/) in om te wijzigen. |
| test | Haalt op of stelt het type vergelijking in dat wordt gemaakt tussen FieldName en Value en dat fungeert als selectiecriterium voor het filter.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Haalt de objectwaarden op om te vergelijken met de waarde van het veld dat is opgegeven met FieldName. |
| criteria_rows | Haalt de lijst op van onderliggende [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) rijen.<br/>            Als het filter meer dan één criteriumrij bevat, is het effect van een EN-operator dat de criteria voor beide rijen moeten worden voldaan zodat de taak of bron wordt weergegeven als resultaat van dit filter.<br/>            Het effect van een OF-operator is dat de criteria voor de ene of de andere rij moeten worden voldaan. |
## Methods
| Naam | Beschrijving |
| :- | :- |
| is_field_value() | Haalt op of de rechterwaarde van FilterCriteria een veldreferentie is, geen constante waarde. |
| set_value_field(value) | Stelt het veld in waarvan de waarde wordt vergeleken met de waarde van het veld dat is opgegeven door FieldName. |

### Zie ook

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

