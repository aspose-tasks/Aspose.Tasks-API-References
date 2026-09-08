---
title: "Enum BaselineType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.BaselineType enum. Geeft het basistype op dat wordt gebruikt om Variance-waarden te berekenen."
type: docs
weight: 130
url: /nl/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Specificeert het basistype dat wordt gebruikt om variantiewaarden te berekenen.

```csharp
public enum BaselineType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft aan dat het veld niet is gedefinieerd in het oorspronkelijke projectbestand. |
| Baseline | `0` | Geeft het basistype aan. |
| Baseline1 | `1` | Geeft het Baseline1-type aan. |
| Baseline2 | `2` | Geeft het Baseline2-type aan. |
| Baseline3 | `3` | Geeft het Baseline3-type aan. |
| Baseline4 | `4` | Geeft het Baseline4-type aan. |
| Baseline5 | `5` | Geeft het Baseline5-type aan. |
| Baseline6 | `6` | Geeft het Baseline6-type aan. |
| Baseline7 | `7` | Geeft het Baseline7-type aan. |
| Baseline8 | `8` | Geeft het Baseline8-type aan. |
| Baseline9 | `9` | Geeft het Baseline9-type aan. |
| Baseline10 | `10` | Geeft het Baseline10-type aan. |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe een baseline voor het project in te stellen (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Sla baseline-velden op naar de opgegeven baseline voor het gehele project.
project.SetBaseline(BaselineType.Baseline);
// Werken met de baselines van het project...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


