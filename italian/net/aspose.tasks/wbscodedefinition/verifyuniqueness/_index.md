---
title: "WBSCodeDefinition.VerifyUniqueness"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà WBSCodeDefinition. Ottiene o imposta un valore che indica se verificare l'unicità dei nuovi codici WBS"
type: docs
weight: 50
url: /it/net/aspose.tasks/wbscodedefinition/verifyuniqueness/
---
## WBSCodeDefinition.VerifyUniqueness property

Ottiene o imposta un valore che indica se verificare l'unicità dei nuovi codici WBS.

```csharp
public bool VerifyUniqueness { get; set; }
```

## Esempi

Mostra come aggiungere maschere di codice WBS.

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

### Vedi anche

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


