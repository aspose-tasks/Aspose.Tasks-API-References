---
title: "क्लास Rate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Rate क्लास। एक समय अवधि की परिभाषा और उस अवधि के दौरान संसाधन पर लागू दरों का प्रतिनिधित्व करता है।"
type: docs
weight: 1610
url: /hi/net/aspose.tasks/rate/
---
## Rate class

उस अवधि के दौरान संसाधन पर लागू समय अवधि और दरों की परिभाषा को दर्शाता है।

```csharp
public class Rate
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | संसाधन के प्रति उपयोग लागत को प्राप्त करता है या सेट करता है। यदि संसाधन के लिए दर तालिका मौजूद है तो यह मान वर्तमान तिथि से प्राप्त किया जाता है। |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | संसाधन के लिए प्रति घंटे ओवरटाइम दर को प्राप्त करता है या सेट करता है। |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Microsoft Project द्वारा ओवरटाइम दर दिखाने के लिए उपयोग किए जाने वाले इकाइयों को प्राप्त करता है या सेट करता है। |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | दर के प्रभावी होने की तिथि को प्राप्त करता है या सेट करता है। |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | दर के प्रभावी रहने की अंतिम तिथि को प्राप्त करता है या सेट करता है। |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | संसाधन के लिए दर तालिका की अद्वितीय पहचानकर्ता को प्राप्त करता है या सेट करता है। |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | संसाधन के लिए प्रति घंटे मानक दर को प्राप्त करता है या सेट करता है। |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Microsoft Project द्वारा मानक दर दिखाने के लिए उपयोग किए जाने वाले इकाइयों को प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


