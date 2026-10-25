---
title: "Class OutlineValue"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.OutlineValue. Représente une valeur d'outline"
type: docs
weight: 1210
url: /fr/net/aspose.tasks/outlinevalue/
---
## OutlineValue class

Représente une valeur de plan.

```csharp
public class OutlineValue
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OutlineValue](outlinevalue/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | Obtient ou définit la description d'une valeur de contour. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | Obtient ou définit la durée si le type est Duration. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | Obtient ou définit une valeur indiquant si la valeur de contour est réduite ou non. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | Obtient ou définit l'Id d'un nœud parent d'un code de contour. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | Obtient ou définit le type de code de contour. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | Obtient ou définit la valeur réelle. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | Obtient un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | Obtient ou définit l'Id unique d'une valeur de code de contour dans un projet. |

## Exemples

Montre comment travailler avec les valeurs d'esquisse.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// créer une valeur d'esquisse
var value = new OutlineValue();

// définir la valeur réelle
value.Value = "Text value 1";

// définir l'ID unique d'une valeur de code d'esquisse dans un projet
value.ValueId = 1;

// obtenir un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// définir le type de code d'esquisse
value.Type = OutlineValueType.Text;

// définir la description d'une valeur d'esquisse
value.Description = "Text value descr 1";

// définir une valeur indiquant si la valeur d'esquisse est réduite ou non
value.IsCollapsed = false;

// vérifier l'ID de la valeur parente
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// créer une valeur d'esquisse avec durée
var value2 = new OutlineValue();

// définir la valeur de durée
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// définir l'ID unique d'une valeur de code d'esquisse dans un projet
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


