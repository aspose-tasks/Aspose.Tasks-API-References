---
title: "WBSCodeDefinition.CodePrefix"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà WBSCodeDefinition. Ottiene o imposta il prefisso del codice progetto"
type: docs
weight: 30
url: /it/net/aspose.tasks/wbscodedefinition/codeprefix/
---
## WBSCodeDefinition.CodePrefix property

Ottiene o imposta il prefisso del codice del progetto.

```csharp
public string CodePrefix { get; set; }
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


