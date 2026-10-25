---
title: "Classe WBSCodeDefinition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WBSCodeDefinition. Rappresenta una definizione di codice WBS"
type: docs
weight: 3490
url: /it/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Rappresenta una definizione di codice WBS.

```csharp
public class WBSCodeDefinition
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Inizializza una nuova istanza della classe `WBSCodeDefinition`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Ottiene la raccolta di oggetti WBSCodeMask. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Ottiene o imposta il prefisso del codice del progetto. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Ottiene o imposta un valore che indica se generare il codice WBS per una nuova attività. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Ottiene o imposta un valore che indica se verificare l'unicità dei nuovi codici WBS. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


