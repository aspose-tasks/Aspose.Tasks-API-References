---
title: "Classe WBSCodeMask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WBSCodeMask. Représente le masque de code WBS"
type: docs
weight: 3500
url: /fr/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Représente le masque de code WBS.

```csharp
public class WBSCodeMask
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Initialise une nouvelle instance de la classe `WBSCodeMask`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Obtient ou définit le nombre de caractères de la chaîne de code. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Obtient le niveau du masque. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Obtient ou définit le séparateur de la chaîne de code. La valeur par défaut est Point. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Obtient ou définit le type de caractère de la chaîne de code. |

## Exemples

Montre comment créer des masques de code WBS.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


