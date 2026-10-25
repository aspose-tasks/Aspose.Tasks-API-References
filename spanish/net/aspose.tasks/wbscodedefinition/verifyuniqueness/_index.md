---
title: "WBSCodeDefinition.VerifyUniqueness"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad WBSCodeDefinition. Obtiene o establece un valor que indica si se debe verificar la unicidad de los nuevos códigos WBS"
type: docs
weight: 50
url: /es/net/aspose.tasks/wbscodedefinition/verifyuniqueness/
---
## WBSCodeDefinition.VerifyUniqueness property

Obtiene o establece un valor que indica si se debe verificar la unicidad de los nuevos códigos WBS.

```csharp
public bool VerifyUniqueness { get; set; }
```

## Ejemplos

Muestra cómo agregar máscaras de código WBS.

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

### Ver también

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


