---
title: "Resource.Delete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource yöntemi. Bir kaynağı ve onun atamalarını projeden siler"
type: docs
weight: 810
url: /tr/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Bir kaynağı ve onun atamalarını projeden siler.

```csharp
public void Delete()
```

## Örnekler

Bir kaynağın nasıl silineceğini gösterir.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// kaynağı sil
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### Ayrıca Bakınız

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


