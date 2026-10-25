---
title: "Sınıf VbaProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.VbaProject sınıfı. VbaProject'i temsil eder."
type: docs
weight: 2860
url: /tr/net/aspose.tasks/vbaproject/
---
## VbaProject class

`VbaProject`'i temsil eder.

```csharp
public class VbaProject
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Koşullu Derleme Argümanlarını alır |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Proje açıklamasını alır. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Proje Yardım Bağlam Kimliğini alır. |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Yardım dosyası adını alır. |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | `[`VbaModuleCollection`](../vbamodulecollection/)` koleksiyonunu alır. |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Proje adını alır. |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | `[`VbaReferenceCollection`](../vbareferencecollection/)` koleksiyonunu alır. |

## Örnekler

VBA proje özelliklerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


