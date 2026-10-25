---
title: "Resource.Rates"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी। इस ऑब्जेक्ट के लिए RateCollection क्लास का एक उदाहरण प्राप्त करता है। प्रत्येक के साथ संबंधित अवधि और दरों का संग्रह।"
type: docs
weight: 640
url: /hi/net/aspose.tasks/resource/rates/
---
## Resource.Rates property

[`RateCollection`](../../ratecollection/) क्लास का एक उदाहरण प्राप्त करता है। प्रत्येक के साथ संबंधित अवधि और दरों का संग्रह।

```csharp
public RateCollection Rates { get; }
```

## उदाहरण

संसाधन दरों को पढ़ने का तरीका दर्शाता है।

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

// दरों पर इटररेट करें
foreach (KeyValuePair<RateType, RateByDateCollection> rate in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in rate.Value)
    {
        Console.WriteLine(pair.Value.RatesFrom);
        Console.WriteLine(pair.Value.RatesTo);
    }
}
```

### संबंधित देखें

* class [RateCollection](../../ratecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


