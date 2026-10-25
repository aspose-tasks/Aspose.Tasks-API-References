---
title: "Rsc.StandardRateFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Microsoft Project'in standart oranı görüntülemek için kullandığı birimler."
type: docs
weight: 630
url: /tr/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Microsoft Project'in standart oranı göstermek için kullandığı birimler.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Örnekler

Rsc.StandardRateFormat özelliğini okuma/yazma işleminin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


