---
title: "Enum RateFormatType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RateFormatType enum. Specificeert de eenheden die Microsoft Project gebruikt om een tarief weer te geven"
type: docs
weight: 1640
url: /nl/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Specificeert de eenheden die Microsoft Project gebruikt om een tarief weer te geven.

```csharp
public enum RateFormatType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | De waarde was niet gedefinieerd in het oorspronkelijke projectbestand. |
| Minute | `0` | Minuut ("min") |
| Hour | `1` | Uur ("hr") |
| Day | `2` | Dag ("day") |
| Week | `3` | Week ("wk") |
| Month | `4` | Maand ("mo") |
| Year | `5` | Jaar ("yr") |
| MaterialResourceRate | `6` | Materiaalresource tarief (leeg) |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe de eigenschap Rsc.StandardRateFormat te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


