---
title: "WBSCodeDefinition.VerifyUniqueness"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WBSCodeDefinition property. Haalt een waarde op of stelt deze in die aangeeft of de uniekheid van nieuwe WBS-codes moet worden geverifieerd"
type: docs
weight: 50
url: /nl/net/aspose.tasks/wbscodedefinition/verifyuniqueness/
---
## WBSCodeDefinition.VerifyUniqueness property

Haalt op of stelt een waarde in die aangeeft of de uniciteit van nieuwe WBS‑codes moet worden geverifieerd.

```csharp
public bool VerifyUniqueness { get; set; }
```

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

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


