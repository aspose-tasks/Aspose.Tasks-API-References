---
title: "Clase WBSCodeMask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WBSCodeMask. Representa una máscara de código WBS"
type: docs
weight: 3500
url: /es/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Representa la máscara de código WBS.

```csharp
public class WBSCodeMask
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Inicializa una nueva instancia de la clase `WBSCodeMask`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Obtiene o establece el número de caracteres de la cadena de código. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Obtiene el nivel de máscara. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Obtiene o establece el separador de la cadena de código. El valor predeterminado es Punto. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Obtiene o establece el tipo de carácter de la cadena de código. |

## Ejemplos

Muestra cómo crear máscaras de código WBS.

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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


