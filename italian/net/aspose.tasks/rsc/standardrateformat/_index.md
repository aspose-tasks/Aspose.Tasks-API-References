---
title: "Rsc.StandardRateFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Le unità utilizzate da Microsoft Project per visualizzare la tariffa standard"
type: docs
weight: 630
url: /it/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Le unità utilizzate da Microsoft Project per visualizzare il tasso standard.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


