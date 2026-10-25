---
title: "Rate.OvertimeRate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Rate. Λαμβάνει ή ορίζει το υπερωριακό ποσοστό ανά ώρα για έναν πόρο"
type: docs
weight: 20
url: /el/net/aspose.tasks/rate/overtimerate/
---
## Rate.OvertimeRate property

Λαμβάνει ή ορίζει το ωριαίο ποσοστό υπερωρίας για έναν πόρο.

```csharp
public decimal OvertimeRate { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργάζεστε με τιμές πόρων.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// εργαστείτε με το έργο...
```

### Δείτε επίσης

* class [Rate](../)
* namespace [Aspose.Tasks](../../rate/)
* assembly [Aspose.Tasks](../../../)


