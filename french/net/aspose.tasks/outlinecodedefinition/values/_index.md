---
title: "OutlineCodeDefinition.Values"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineCodeDefinition propriété. Obtient l'objet OutlineValueCollection. Les valeurs du tableau associé à ce code de contour"
type: docs
weight: 150
url: /fr/net/aspose.tasks/outlinecodedefinition/values/
---
## OutlineCodeDefinition.Values property

Obtient l'objet OutlineValueCollection. Les valeurs du tableau associées à ce code de contour.

```csharp
public OutlineValueCollection Values { get; }
```

## Exemples

Montre comment créer de nouveaux codes de contour.

```csharp
var project = new Project(DataDir + "project.mpp");

// Définir le code de contour et son masque de contour
var code1 = new OutlineCodeDefinition();
code1.Alias = "New task outline code1";
code1.FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString();
code1.FieldName = "Outline Code1";
var mask = new OutlineMask();
mask.Separator = "+";
mask.Level = 1;
mask.Type = MaskType.Numbers;
code1.Masks.Add(mask);

// Ajouter une valeur de contour
var value = new OutlineValue();
value.Description = "Value description";
value.ValueId = 1;
value.Value = "123456";
value.Type = OutlineValueType.Number;
code1.Values.Add(value);

// Ajouter le code de contour au projet
project.OutlineCodes.Add(code1);

// Définir le code de contour et son masque de contour
var code2 = new OutlineCodeDefinition();
code2.Alias = "New rsc outline code2";
code2.FieldId = ((int)ExtendedAttributeResource.OutlineCode2).ToString();
code2.FieldName = "Outline Code2";
var mask2 = new OutlineMask();
mask2.Separator = "/";
mask2.Level = 1;
mask2.Type = MaskType.Numbers;
code2.Masks.Add(mask2);

// Ajouter une valeur de contour
var value2 = new OutlineValue();
value2.Description = "Value2 description";
value2.ValueId = 2;
value2.Value = "987654";
value2.Type = OutlineValueType.Number;
code2.Values.Add(value2);

// Ajouter le code de contour au projet
project.OutlineCodes.Add(code2);

project.Save(OutDir + "Updated_project_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [OutlineValueCollection](../../outlinevaluecollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


