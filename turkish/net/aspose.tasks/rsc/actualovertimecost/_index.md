---
title: "Rsc.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Atanan kaynaklar tarafından görevlerde zaten yapılan fazla mesai çalışması için oluşan maliyetler"
type: docs
weight: 40
url: /tr/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Atanan kaynaklar tarafından görevlerde zaten yapılan fazla mesai çalışması için oluşan maliyetler.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Örnekler

Rsc.ActualOvertimeCost özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


