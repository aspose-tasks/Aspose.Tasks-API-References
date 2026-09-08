---
title: "Clase WBSCodeDefinition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WBSCodeDefinition. Representa una definición de código WBS"
type: docs
weight: 3490
url: /es/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Representa una definición de código WBS.

```csharp
public class WBSCodeDefinition
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Inicializa una nueva instancia de la clase `WBSCodeDefinition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Obtiene la colección de objetos WBSCodeMask. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Obtiene o establece el prefijo del código del proyecto. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Obtiene o establece un valor que indica si se debe generar código WBS para una nueva tarea. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Obtiene o establece un valor que indica si se debe verificar la unicidad de los nuevos códigos WBS. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


