---
title: "Enumeración WBSSequence"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.WBSSequence enum. Especifica la secuencia para WBSCodeMask"
type: docs
weight: 3520
url: /es/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Especifica la secuencia para WBSCodeMask

```csharp
public enum WBSSequence
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| OrderedNumbers | `0` | Indica la secuencia de números WBS. |
| OrderedUppercaseLetters | `1` | Indica la secuencia de letras mayúsculas WBS. |
| OrderedLowercaseLetters | `2` | Indica la secuencia de letras minúsculas WBS. |
| UnorderedCharacters | `3` | Indica la secuencia de caracteres desordenados WBS. |

## Ejemplos

Muestra cómo establecer secuencias WBS.

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


