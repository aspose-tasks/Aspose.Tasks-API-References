---
title: "Rsc.ActualCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kaynakların görevlerinde zaten gerçekleştirdiği çalışmalar için ortaya çıkan maliyetler ve görevle ilişkili diğer kaydedilmiş maliyetler."
type: docs
weight: 30
url: /tr/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Kaynakların görevlerinde zaten gerçekleştirdiği işler için oluşan maliyetler ve görevle ilişkili diğer kaydedilmiş maliyetler.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Örnekler

Rsc.ActualCost özelliğini nasıl okuyup yazacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


