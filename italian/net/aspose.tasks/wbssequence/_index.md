---
title: "Enum WBSSequence"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.WBSSequence. Specifica la sequenza per WBSCodeMask"
type: docs
weight: 3520
url: /it/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Specifica la sequenza per WBSCodeMask

```csharp
public enum WBSSequence
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| OrderedNumbers | `0` | Indica la sequenza WBS numerica. |
| OrderedUppercaseLetters | `1` | Indica la sequenza WBS di lettere maiuscole. |
| OrderedLowercaseLetters | `2` | Indica la sequenza WBS di lettere minuscole. |
| UnorderedCharacters | `3` | Indica la sequenza WBS di caratteri non ordinati. |

## Esempi

Mostra come impostare le sequenze WBS.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


