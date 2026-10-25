---
title: "Rsc.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Gerçek işin korunduğu iş miktarı."
type: docs
weight: 80
url: /tr/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

Gerçek işin korunduğu iş miktarı.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Örnekler

Rsc.ActualWorkProtected özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


