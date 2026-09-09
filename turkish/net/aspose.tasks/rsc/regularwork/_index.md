---
title: "Rsc.RegularWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kaynak tarafından yapılması planlanan fazla mesai dışı toplam iş miktarı."
type: docs
weight: 570
url: /tr/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

Kaynak tarafından yapılması planlanan fazla mesai dışı işin toplam miktarı.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Örnekler

Rsc.RegularWork özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


