---
title: "Classe OutlineMask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.OutlineMask. Représente quatre éléments d'un masque qui définit un format de code de contour"
type: docs
weight: 1190
url: /fr/net/aspose.tasks/outlinemask/
---
## OutlineMask class

Représente les quatre éléments d'un masque qui définit le format d'un code de plan.

```csharp
public class OutlineMask
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OutlineMask](outlinemask/)() | Initialise une nouvelle instance de la classe `OutlineMask`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Obtient ou définit la longueur maximale (en caractères) des valeurs du code de contour. 0 si la longueur n'est pas définie. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Obtient ou définit le niveau d'un masque. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Obtient ou définit le séparateur des valeurs de code. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Obtient ou définit le type d'un masque. |

## Exemples

Montre comment travailler avec les masques de contour.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// définir le type d'un masque
mask.Type = MaskType.Characters;

// définir le séparateur des valeurs de code
mask.Separator = "/";

// définir le niveau d'un masque
mask.Level = 1;

// définir la longueur maximale (en caractères) des valeurs de code de contour. 0 si la longueur n'est pas définie.
mask.Length = 2;

// ajouter le masque à la définition
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


