---
title: "Rsc.Finish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın atanan tüm görevlerde çalışmayı tamamlaması planlanan tarih."
type: docs
weight: 290
url: /tr/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

Bir kaynağın tüm atanan görevlerdeki işi tamamlaması planlanan tarih.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Örnekler

Rsc.Finish özelliğini nasıl okuyup yazacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


