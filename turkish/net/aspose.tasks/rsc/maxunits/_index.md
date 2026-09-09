---
title: "Rsc.MaxUnits"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın mevcut olduğu ve mevcut zaman diliminde herhangi bir görevi yerine getirebileceği maksimum kapasiteyi temsil eden birimlerin maksimum sayısı"
type: docs
weight: 450
url: /tr/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

Kaynağın mevcut zaman diliminde herhangi bir görevi yerine getirebilmesi için mevcut olduğu maksimum kapasiteyi temsil eden birimlerin en fazla sayısı.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Örnekler

Rsc.MaxUnits özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


