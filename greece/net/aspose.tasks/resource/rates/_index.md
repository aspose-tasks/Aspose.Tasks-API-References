---
title: "Resource.Rates"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει το στιγμιότυπο της κλάσης RateCollection για αυτό το αντικείμενο. Η συλλογή των περιόδων και των ρυθμών που σχετίζονται με το καθένα"
type: docs
weight: 640
url: /el/net/aspose.tasks/resource/rates/
---
## Resource.Rates property

Λαμβάνει το στιγμιότυπο της κλάσης [`RateCollection`](../../ratecollection/) για αυτό το αντικείμενο. Η συλλογή των περιόδων και των ρυθμών που σχετίζονται με το καθένα.

```csharp
public RateCollection Rates { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους ρυθμούς του πόρου.

```csharp
var project = new Project();
var resource = project.Resources.Add();
resource.Set(Rsc.Uid, 1);
resource.Set(Rsc.Name, "Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

// επανάληψη στους ρυθμούς
foreach (KeyValuePair<RateType, RateByDateCollection> rate in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in rate.Value)
    {
        Console.WriteLine(pair.Value.RatesFrom);
        Console.WriteLine(pair.Value.RatesTo);
    }
}
```

### Δείτε επίσης

* class [RateCollection](../../ratecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


