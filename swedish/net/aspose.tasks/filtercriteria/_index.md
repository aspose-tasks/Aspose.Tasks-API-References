---
title: Class FilterCriteria
second_title: Aspose.Tasks för .NET API-referens
description: Aspose.Tasks.FilterCriteria klass. Definierar kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSPvy.
type: docs
weight: 630
url: /sv/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Definierar kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP-vy.

```csharp
public class FilterCriteria
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Hämtar listan över barn`FilterCriteria` rows. Om filtret innehåller mer än en kriterierad är effekten av en And-operator att kriterierna för båda raderna måste uppfyllas för att uppgiften eller resursen ska visas som ett resultat av detta filter. Effekten av en Or operatorn är att kriterierna för den ena eller andra raden måste uppfyllas. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Hämtar eller sätter en[`Field`](./field/) att ändra. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Hämtar eller ställer in kriteriet som fastställts med FieldName, Test och Value relaterar till andra kriterier i filtret. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Hämtar eller ställer in den typ av jämförelse som görs mellan Fältnamn och Värde som fungerar som urvalskriterier för filtret. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Hämtar objektvärdena att jämföra med värdet för fältet som anges med FieldName. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Returnerar strängrepresentation av instansen av`FilterCriteria` class. |

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks/)
* hopsättning [Aspose.Tasks](../../)


