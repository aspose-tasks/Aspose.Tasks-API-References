---
title: "Rsc.AvailableTo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın mevcut zaman dilimi için belirtilen birimlerde çalışmaya uygun olduğu son tarih."
type: docs
weight: 130
url: /tr/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

Kaynağın mevcut zaman dilimi için belirtilen birimlerde çalışmaya uygun olduğu bitiş tarihi.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Örnekler

Rsc.AvailableTo özelliğini nasıl okuyup yazacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


