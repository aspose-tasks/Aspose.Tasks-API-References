---
title: "AvailabilityPeriod.AvailableTo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AvailabilityPeriod प्रॉपर्टी। प्राप्त करता है या सेट करता है अंतिम तिथि जब संसाधन निर्दिष्ट अवधि के लिए उपलब्ध है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/availabilityperiod/availableto/
---
## AvailabilityPeriod.AvailableTo property

निर्दिष्ट अवधि के लिए जब संसाधन उपलब्ध हो, उसकी अंतिम तिथि प्राप्त करता है या सेट करता है।

```csharp
public DateTime AvailableTo { get; set; }
```

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

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


