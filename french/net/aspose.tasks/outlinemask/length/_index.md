---
title: "OutlineMask.Length"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété OutlineMask. Obtient ou définit la longueur maximale en caractères des valeurs de code de contour. 0 si la longueur n'est pas définie"
type: docs
weight: 20
url: /fr/net/aspose.tasks/outlinemask/length/
---
## OutlineMask.Length property

Obtient ou définit la longueur maximale (en caractères) des valeurs du code de contour. 0 si la longueur n'est pas définie.

```csharp
public int Length { get; set; }
```

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

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


