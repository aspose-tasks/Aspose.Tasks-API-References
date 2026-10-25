---
title: "Rsc.StandardRateFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De eenheden die door Microsoft Project worden gebruikt om het standaardtarief weer te geven."
type: docs
weight: 630
url: /nl/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

De eenheden die Microsoft Project gebruikt om het standaardtarief weer te geven.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.StandardRateFormat te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


