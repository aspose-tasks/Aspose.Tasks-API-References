---
title: "Enum CurrencySymbolPositionType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CurrencySymbolPositionType enum. Specificeert de positie van een valutasymbool"
type: docs
weight: 370
url: /nl/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Specificeert de positie van een valutasymbool.

```csharp
public enum CurrencySymbolPositionType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft aan dat een ongedefinieerde waarde betekent dat het veld niet gedefinieerd was in het oorspronkelijke projectbestand. |
| Before | `0` | Geeft het type positie vóór het valutasymbool aan. |
| After | `1` | Geeft het type positie na het valutasymbool aan. |
| BeforeWithSpace | `2` | Geeft het type positie vóór met spatie van het valutasymbool aan. |
| AfterWithSpace | `3` | Geeft het type positie na met spatie van het valutasymbool aan. |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe de plaatsing van het valutasymbool op te geven (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// stel de plaatsing van het valutasymbool in
// Voor, geen spatie ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// werken met het project...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


