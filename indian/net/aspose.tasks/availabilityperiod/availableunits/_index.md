---
title: "AvailabilityPeriod.AvailableUnits"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AvailabilityPeriod प्रॉपर्टी। प्राप्त करता है या सेट करता है प्रतिशत जो संसाधन निर्दिष्ट अवधि के दौरान उपलब्ध है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/availabilityperiod/availableunits/
---
## AvailabilityPeriod.AvailableUnits property

निर्दिष्ट अवधि के दौरान उपलब्ध संसाधन का प्रतिशत प्राप्त करता है या सेट करता है।

```csharp
public double AvailableUnits { get; set; }
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


