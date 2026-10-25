---
title: "Rsc.Work"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir görevde bir kaynak için planlanan toplam süre."
type: docs
weight: 690
url: /tr/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

Bir görevde bir kaynak için planlanan toplam zaman miktarı.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Örnekler

Rsc.Work özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


