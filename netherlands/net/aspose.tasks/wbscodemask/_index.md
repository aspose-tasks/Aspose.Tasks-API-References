---
title: "Klasse WBSCodeMask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WBSCodeMask‑klasse. Vertegenwoordigt een WBS‑codemasker."
type: docs
weight: 3500
url: /nl/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Stelt WBS Code mask voor.

```csharp
public class WBSCodeMask
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Initialiseert een nieuw exemplaar van de `WBSCodeMask`‑klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Haalt op of stelt het aantal tekens van de code‑reeks in. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Haalt het maskerniveau op. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Haalt de scheidingsteken van de code‑reeks op of stelt deze in. Standaardwaarde is Punt. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Haalt het type teken van de code‑reeks op of stelt dit in. |

## Voorbeelden

Toont hoe WBS‑codemaskers te maken.

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

var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

project.Recalculate();

Console.WriteLine("Number of WBS masks: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
var i = 0;
foreach (var cm in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("WBS Mask #{0}: Level->{1}", ++i, cm.Level);
}

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


