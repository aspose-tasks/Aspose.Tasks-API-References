---
title: "Enum WBSSequence"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.WBSSequence. Spécifie la séquence pour WBSCodeMask"
type: docs
weight: 3520
url: /fr/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Spécifie la séquence pour WBSCodeMask

```csharp
public enum WBSSequence
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| OrderedNumbers | `0` | Indique la séquence WBS numérique. |
| OrderedUppercaseLetters | `1` | Indique la séquence WBS des lettres majuscules. |
| OrderedLowercaseLetters | `2` | Indique la séquence WBS des lettres minuscules. |
| UnorderedCharacters | `3` | Indique la séquence WBS des caractères non ordonnés. |

## Exemples

Montre comment définir les séquences WBS.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


