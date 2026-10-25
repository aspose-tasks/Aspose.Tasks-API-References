---
title: "Rsc.Start"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Atanan bir kaynağın bir göreve çalışmaya başlaması planlanan tarih"
type: docs
weight: 640
url: /tr/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

Atanan bir kaynağın bir görevde çalışmaya başlaması planlanan tarih.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Örnekler

Rsc.Start özelliğini nasıl okuma/yazma yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


