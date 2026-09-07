---
title: "क्लास RateCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RateCollection क्लास। एक संग्रह का प्रतिनिधित्व करता है जिसमें Rate ऑब्जेक्ट्स होते हैं।"
type: docs
weight: 1630
url: /hi/net/aspose.tasks/ratecollection/
---
## RateCollection class

एक संग्रह का प्रतिनिधित्व करता है जिसमें [`Rate`](../rate/) ऑब्जेक्ट्स होते हैं।

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | RateCollection में शामिल तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है। |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | इस संग्रह के लिए पैरेंट [`Resource`](../resource/) ऑब्जेक्ट प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | इस संग्रह में एक नया [`Rate`](../rate/) इंस्टेंस जोड़ता है। |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | इस संग्रह में एक नया [`Rate`](../rate/) इंस्टेंस जोड़ता है। |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | इस संग्रह से Rate इंस्टेंस हटाता है। |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | `RateCollection` ऑब्जेक्ट को [`Rate`](../rate/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | `RateCollection` ऑब्जेक्ट को निर्दिष्ट [`RateType`](../ratetype/) प्रकार द्वारा फ़िल्टर किए गए [`Rate`](../rate/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

दर संग्रहों के साथ काम करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0), RateType.B);
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

Console.WriteLine("Print rates of '{0}' resource: ", resource.Rates.ParentResource.Get(Rsc.Name));
Console.WriteLine("Count of rates: {0}", resource.Rates.Count);
Console.WriteLine("Is rate collection read-only: {0}", resource.Rates.IsReadOnly);
foreach (KeyValuePair<RateType, RateByDateCollection> sortedRates in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in sortedRates.Value)
    {
        var rate = pair.Value;
        Console.WriteLine("Rates From: " + rate.RatesFrom);
        Console.WriteLine("Rates To: " + rate.RatesTo);
        Console.WriteLine("Rate Table: " + rate.RateTable);
        Console.WriteLine();
    }
}

// इंडेक्स एक्सेस द्वारा नवीनतम दर प्राप्त करें
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// दरों के साथ काम करें
// ...

// प्रकार A की सभी दरें हटाएँ
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// दर संग्रह को एक फ्लैट सूची में बदलें
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### संबंधित देखें

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


