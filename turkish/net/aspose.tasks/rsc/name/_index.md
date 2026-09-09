---
title: "Rsc.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın adı"
type: docs
weight: 460
url: /tr/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

Bir kaynağın adı.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Örnekler

Rsc.Name özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


