---
title: "Rsc.RemainingCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kalan planlı işi tamamlamada ortaya çıkacak kalan planlı gider"
type: docs
weight: 580
url: /tr/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

Kalan planlı işi tamamlamada ortaya çıkacak kalan planlı gider.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Örnekler

Rsc.RemainingCost özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


