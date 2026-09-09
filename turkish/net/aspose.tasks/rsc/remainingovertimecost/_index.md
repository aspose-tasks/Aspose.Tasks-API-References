---
title: "Rsc.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynak için kalan planlanmış fazla mesai gideri."
type: docs
weight: 590
url: /tr/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

Bir kaynak için kalan planlı fazla mesai gideri.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Örnekler

Rsc.RemainingOvertimeCost özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


