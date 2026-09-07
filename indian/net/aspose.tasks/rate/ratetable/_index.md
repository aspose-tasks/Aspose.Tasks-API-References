---
title: "Rate.RateTable"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rate प्रॉपर्टी। किसी संसाधन के लिए रेट टेबल का अद्वितीय पहचानकर्ता प्राप्त करती या सेट करती है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/rate/ratetable/
---
## Rate.RateTable property

संसाधन के लिए दर तालिका की अद्वितीय पहचानकर्ता को प्राप्त करता है या सेट करता है।

```csharp
public RateType RateTable { get; set; }
```

## उदाहरण

दिखाता है कि संसाधन दरों के साथ कैसे काम करें।

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

// परियोजना के साथ काम करें...
```

### संबंधित देखें

* enum [RateType](../../ratetype/)
* class [Rate](../)
* namespace [Aspose.Tasks](../../rate/)
* assembly [Aspose.Tasks](../../../)


