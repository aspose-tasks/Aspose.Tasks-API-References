---
title: "Resource.ParentProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource özelliği. Bu kapsayıcı için üst projeyi alır."
type: docs
weight: 600
url: /tr/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Bu kapsayıcı için üst projeyi alır.

```csharp
public Project ParentProject { get; }
```

## Örnekler

Kaynağın üst projesinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// Kaynak için varsayılan proje çalışma zaman birimi türünü kullanarak bir iş ayarlayın.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### Ayrıca Bakınız

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


