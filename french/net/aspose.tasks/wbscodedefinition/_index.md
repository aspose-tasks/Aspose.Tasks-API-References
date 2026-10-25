---
title: "Classe WBSCodeDefinition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WBSCodeDefinition. Représente une définition de code WBS."
type: docs
weight: 3490
url: /fr/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Représente une définition de code WBS.

```csharp
public class WBSCodeDefinition
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Initialise une nouvelle instance de la classe `WBSCodeDefinition`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Obtient la collection d'objets WBSCodeMask. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Obtient ou définit le préfixe du code du projet. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut générer un code WBS pour une nouvelle tâche. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut vérifier l'unicité des nouveaux codes WBS. |

## Exemples

Montre comment ajouter des masques de code WBS.

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


