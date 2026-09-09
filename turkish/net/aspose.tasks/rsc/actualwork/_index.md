---
title: "Rsc.ActualWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Görevlere atanan kaynak tarafından zaten yapılan iş miktarı"
type: docs
weight: 70
url: /tr/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

Görevlere atanan kaynak tarafından zaten yapılan iş miktarı.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Örnekler

Rsc.ActualWork özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


