---
title: Resource.Rates
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets a the instance of the RateCollection class for this object. The collection of periods and rates associated with each one
type: docs
weight: 640
url: /net/aspose.tasks/resource/rates/
---
## Resource.Rates property

Gets a the instance of the [`RateCollection`](../../ratecollection/) class for this object. The collection of periods and rates associated with each one.

```csharp
public RateCollection Rates { get; }
```

## Examples

Shows how to read resource rates.

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

// iterate over rates
foreach (KeyValuePair<RateType, RateByDateCollection> rate in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in rate.Value)
    {
        Console.WriteLine(pair.Value.RatesFrom);
        Console.WriteLine(pair.Value.RatesTo);
    }
}
```

### See Also

* class [RateCollection](../../ratecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


