---
title: "Project.GetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projectmethode. Retourneert de baseline-opslagtijd"
type: docs
weight: 1090
url: /nl/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Retourneert de baseline-opslagtijd.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| baselineNumber | BaselineType | Het nummer van de baseline [`BaselineType`](../../baselinetype/). |

### Retourwaarde

De laatste opslagdatum en -tijd van de baseline.

## Opmerkingen

Retourneert DateTime.MinValue als de baseline niet is opgeslagen.

## Voorbeelden

Toont hoe de baseline‑opslagtijd van het project gelezen/schreven kan worden.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// stel baseline‑opslagtijd in
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### Zie ook

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


