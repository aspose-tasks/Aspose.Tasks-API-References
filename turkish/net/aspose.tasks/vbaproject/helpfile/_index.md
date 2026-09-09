---
title: "VbaProject.HelpFile"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaProject özelliği. Bir yardım dosyası adını alır"
type: docs
weight: 40
url: /tr/net/aspose.tasks/vbaproject/helpfile/
---
## VbaProject.HelpFile property

Yardım dosyası adını alır.

```csharp
public string HelpFile { get; }
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


