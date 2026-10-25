---
title: "Rsc.AvailableFrom"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın mevcut zaman dilimi için belirtilen birimlerde çalışmaya uygun olduğu başlangıç tarihi."
type: docs
weight: 120
url: /tr/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

Kaynağın mevcut zaman dilimi için belirtilen birimlerde çalışmaya uygun olduğu başlangıç tarihi.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Örnekler

Rsc.AvailableFrom özelliğini nasıl okuyup yazacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


