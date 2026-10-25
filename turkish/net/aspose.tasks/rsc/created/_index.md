---
title: "Rsc.Created"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın projeye eklendiği tarih ve saat."
type: docs
weight: 260
url: /tr/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

Bir kaynağın projeye eklendiği tarih ve saat.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Örnekler

Rsc.Created özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


