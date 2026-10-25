---
title: "VbaProject.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaProject özelliği. Proje adını alır"
type: docs
weight: 60
url: /tr/net/aspose.tasks/vbaproject/name/
---
## VbaProject.Name property

Proje adını alır.

```csharp
public string Name { get; }
```

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

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


