---
title: "Klasse WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WBSCodeDefinition klasse. Vertegenwoordigt een WBS‑code‑definitie"
type: docs
weight: 3490
url: /nl/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Stelt een WBS Code Definition voor.

```csharp
public class WBSCodeDefinition
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Initialiseert een nieuw exemplaar van de `WBSCodeDefinition` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Verkrijgt de verzameling van WBSCodeMask‑objecten. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Haalt op of stelt het projectcode‑voorvoegsel in. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of WBS‑code moet worden gegenereerd voor een nieuwe taak. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de uniciteit van nieuwe WBS‑codes moet worden geverifieerd. |

## Voorbeelden

Toont hoe WBS‑code‑maskers toe te voegen.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


