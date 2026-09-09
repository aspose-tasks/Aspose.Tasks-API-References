---
title: "VbaProject.CompilationArguments"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaProject özelliği. Koşullu Derleme Argümanlarını alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/vbaproject/compilationarguments/
---
## VbaProject.CompilationArguments property

Koşullu Derleme Argümanlarını alır

```csharp
public string CompilationArguments { get; }
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


