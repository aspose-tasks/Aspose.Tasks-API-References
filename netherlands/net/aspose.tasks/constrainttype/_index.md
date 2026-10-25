---
title: "Enum ConstraintType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ConstraintType enum. Specificeert de beperking op de start- of einddatum van een taak"
type: docs
weight: 330
url: /nl/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Specificeert de beperking op de start- of einddatum van een taak.

```csharp
public enum ConstraintType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | De waarde was niet gedefinieerd in het oorspronkelijke projectbestand. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) en [`Finish`](../tsk/finish/) data van [`Task`](../task/) worden zo snel mogelijk gepland ten opzichte van de bovenliggende [`Start`](../tsk/start/) en [`Finish`](../tsk/finish/) data, rekening houdend met [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) en [`Finish`](../tsk/finish/) data van [`Task`](../task/) zijn gepland ALAP met betrekking tot de bovenliggende [`Start`](../tsk/start/) en [`Finish`](../tsk/finish/) data en rekening houdend met [`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | Moet starten op |
| MustFinishOn | `3` | Moet eindigen op |
| StartNoEarlierThan | `4` | Start niet eerder dan |
| StartNoLaterThan | `5` | Start niet later dan |
| FinishNoEarlierThan | `6` | Eind niet eerder dan |
| FinishNoLaterThan | `7` | Eind niet later dan |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe je de constraint &lt;see cref="Aspose.Tasks.ConstraintType" /&gt; ConstraintType.AsSoonAsPossible constraint voor een taak instelt.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Stel constraint As Soon As Possible in voor taak met Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


