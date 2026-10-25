---
title: "Sınıf VbaModule"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.VbaModule sınıfı. Bir VBA modülünü temsil eder"
type: docs
weight: 2810
url: /tr/net/aspose.tasks/vbamodule/
---
## VbaModule class

Bir VBA modülünü temsil eder.

```csharp
public sealed class VbaModule
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Modülün özniteliklerinin bir koleksiyonunu alır. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | VBA modülünün adını alır |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | VBA modülünün kaynak kodunu alır veya ayarlar |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Modülün tipini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | `VbaModule` sınıfının VbaModuleType.ClassModule türüyle bir örneğini oluşturur. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | `VbaModule` sınıfının VbaModuleType.ProceduralModule türüyle bir örneğini oluşturur. |

## Örnekler

VBA projesinin modüllerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


