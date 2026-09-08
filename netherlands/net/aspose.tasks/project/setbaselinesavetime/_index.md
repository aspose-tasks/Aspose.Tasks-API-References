---
title: "Project.SetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project methode. Stelt de baseline‑opslagtijd in."
type: docs
weight: 1260
url: /nl/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Stelt de baseline-opslagtijd in.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| baselineNumber | BaselineType | Het nummer van de baseline [`BaselineType`](../../baselinetype/). |
| value | DateTime | De laatste opslagdatum en -tijd van de baseline. |

## Opmerkingen

Stel de waarde in op DateTime.MinValue als de baseline niet is opgeslagen.

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


