---
title: "FilterCriteria"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 350
url: /sv/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Definierar kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP-vyn.

Typen FilterCriteria exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| FilterCriteria() | Initierar en ny instans av klassen FilterCriteria |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| operation | Hämtar eller anger kriteriet som fastställts med FieldName, Test och Value och som relaterar till andra kriterier i filtret. |
| field | Hämtar eller anger ett [field](/tasks/python-net/aspose.tasks/filtercriteria/) att ändra. |
| test | Hämtar eller anger typen av jämförelse som görs mellan FieldName och Value och som fungerar som urvalskriterium för filtret.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Hämtar objektvärdena för att jämföra med värdet på fältet som anges med FieldName. |
| criteria_rows | Hämtar listan över underordnade [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) rader.<br/>            Om filtret innehåller mer än en kriterierad rad innebär en AND-operator att kriterierna för båda raderna måste uppfyllas för att uppgiften eller resursen ska visas som ett resultat av detta filter.<br/>            En OR-operator innebär att kriterierna för den ena eller den andra raden måste uppfyllas. |
## Methods
| Namn | Beskrivning |
| :- | :- |
| is_field_value() | Hämtar om det högra värdet i FilterCriteria är en fältreferens, inte ett konstantvärde. |
| set_value_field(value) | Anger fältet vars värde kommer att jämföras med värdet på fältet som anges av FieldName. |

### Se även

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

