---
title: "Classe WBSCodeMask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WBSCodeMask. Rappresenta la maschera del codice WBS"
type: docs
weight: 3500
url: /it/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Rappresenta la maschera del codice WBS.

```csharp
public class WBSCodeMask
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Inizializza una nuova istanza della classe `WBSCodeMask`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Ottiene o imposta il numero di caratteri della stringa del codice. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Ottiene il livello della maschera. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Ottiene o imposta il separatore della stringa di codice. Il valore predefinito è Punto. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Ottiene o imposta il tipo di carattere della stringa di codice. |

## Esempi

Mostra come creare maschere di codice WBS.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


