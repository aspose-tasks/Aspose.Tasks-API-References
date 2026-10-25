---
title: "Project.WBSCodeDefinition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene o establece WBS Code Definition para el proyecto"
type: docs
weight: 1030
url: /es/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

Obtiene o establece la definición de WBS Code Definition para el proyecto.

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## Ejemplos

Muestra cómo agregar códigos WBS.

```csharp
var project = new Project
{
    WBSCodeDefinition = new WBSCodeDefinition()
};
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask
{
    Length = 2,
    Separator = "-",
    Sequence = WBSSequence.OrderedNumbers
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask
{
    Length = 1,
    Separator = "-",
    Sequence = WBSSequence.OrderedUppercaseLetters
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Ver también

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


