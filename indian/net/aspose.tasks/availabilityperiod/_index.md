---
title: "क्लास AvailabilityPeriod"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.AvailabilityPeriod क्लास. एक अवधि का प्रतिनिधित्व करता है जब संसाधन उपलब्ध होता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

संसाधन उपलब्ध होने की अवधि को दर्शाता है।

```csharp
public class AvailabilityPeriod
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | `AvailabilityPeriod` का एक नया उदाहरण प्रारंभ करता है। |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | `AvailabilityPeriod` का एक नया उदाहरण निर्दिष्ट तिथि सीमा और उपलब्ध इकाइयों के साथ प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | निर्दिष्ट अवधि के लिए जब संसाधन उपलब्ध हो जाता है, उसकी तिथि प्राप्त करता है या सेट करता है। |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | निर्दिष्ट अवधि के लिए जब संसाधन उपलब्ध हो, उसकी अंतिम तिथि प्राप्त करता है या सेट करता है। |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | निर्दिष्ट अवधि के दौरान उपलब्ध संसाधन का प्रतिशत प्राप्त करता है या सेट करता है। |

## उदाहरण

दिखाता है कि संसाधन के लिए उपलब्धता अवधि कैसे बनाई जाए।

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // नए संसाधन में उपलब्धता अवधि जोड़ें
    IEnumerable<AvailabilityPeriod> periods = GetPeriods();
    foreach (var period in periods)
    {
        resource.AvailabilityPeriods.Add(period);
    }

    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private static IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>(2);
    var period = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2011, 12, 12),
        AvailableTo = new DateTime(2013, 12, 12),
        AvailableUnits = 0.99
    };

    periods.Add(period);

    var period2 = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2013, 12, 12),
        AvailableTo = new DateTime(2015, 12, 12),
        AvailableUnits = 0.94
    };
    periods.Add(period2);
    return periods;
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


