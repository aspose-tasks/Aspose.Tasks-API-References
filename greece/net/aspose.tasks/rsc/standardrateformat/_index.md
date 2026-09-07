---
title: "Rsc.StandardRateFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ρυθμού"
type: docs
weight: 630
url: /el/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του τυπικού ρυθμού.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


