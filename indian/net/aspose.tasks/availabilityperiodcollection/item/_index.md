---
title: "AvailabilityPeriodCollection.Item"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AvailabilityPeriodCollection प्रॉपर्टी। निर्दिष्ट इंडेक्स पर तत्व को प्राप्त या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/availabilityperiodcollection/item/
---
## AvailabilityPeriodCollection indexer

निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है।

```csharp
public AvailabilityPeriod this[int index] { get; set; }
```

| पैरामीटर | विवरण |
| --- | --- |
| इंडेक्स | प्राप्त या सेट करने वाले तत्व का शून्य-आधारित अनुक्रमणिका। |

### रिटर्न वैल्यू

निर्दिष्ट अनुक्रमणिका पर तत्व।

## उदाहरण

संसाधन की उपलब्धता अवधि संग्रह के साथ काम करने का तरीका दिखाता है।

```csharp
public void WorkWithAvailabilityPeriodCollection()
{
    var project = new Project(DataDir + "UpdateResourceData.mpp");
    var resource = project.Resources.GetById(1);

    resource.AvailabilityPeriods.Clear();

    // नए संसाधन में उपलब्धता अवधियों (2012 और 2014 वर्ष) को जोड़ें
    IEnumerable<AvailabilityPeriod> periods = this.GetPeriods();
    foreach (var period in periods)
    {
        if (!resource.AvailabilityPeriods.IsReadOnly)
        {
            resource.AvailabilityPeriods.Add(period);
        }
    }

    var period2013 = new AvailabilityPeriod { AvailableFrom = new DateTime(2013, 1, 1), AvailableTo = new DateTime(2013, 12, 12), AvailableUnits = 0.81 };

    if (!resource.AvailabilityPeriods.Contains(period2013))
    {
        resource.AvailabilityPeriods.Insert(1, period2013);
    }

    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }

    var periodsToCopy = new AvailabilityPeriod[resource.AvailabilityPeriods.Count];
    resource.AvailabilityPeriods.CopyTo(periodsToCopy, 0);

    var otherResource = project.Resources.GetById(2);
    otherResource.AvailabilityPeriods.Clear();
    foreach (var period in periodsToCopy)
    {
        otherResource.AvailabilityPeriods.Add(period);
    }

    var period2015 = new AvailabilityPeriod { AvailableFrom = new DateTime(2015, 1, 1), AvailableTo = new DateTime(2015, 12, 12), AvailableUnits = 0.50 };

    var period2016 = new AvailabilityPeriod { AvailableFrom = new DateTime(2016, 1, 1), AvailableTo = new DateTime(2016, 12, 12), AvailableUnits = 0.53 };

    if (otherResource.AvailabilityPeriods.IndexOf(period2015) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2015);
    }

    if (otherResource.AvailabilityPeriods.IndexOf(period2016) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2016);
    }

    // 2014 वर्ष की अवधि के लिए उपलब्ध इकाइयों को अपडेट करें
    otherResource.AvailabilityPeriods[otherResource.AvailabilityPeriods.Count - 2].AvailableUnits = 0.90;

    // 2013 की अवधि को हटाएँ
    otherResource.AvailabilityPeriods.Remove(period2013);

    // 2011 की अवधि को हटाएँ
    otherResource.AvailabilityPeriods.RemoveAt(0);

    Console.WriteLine("Print resource availability periods of the resource: " + otherResource.Get(Rsc.Name));
    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>();
    var period = new AvailabilityPeriod { AvailableFrom = new DateTime(2012, 1, 1), AvailableTo = new DateTime(2012, 12, 12), AvailableUnits = 0.99 };
    periods.Add(period);

    var period2 = new AvailabilityPeriod { AvailableFrom = new DateTime(2014, 1, 1), AvailableTo = new DateTime(2014, 12, 12), AvailableUnits = 0.94 };
    periods.Add(period2);
    return periods;
}
```

### संबंधित देखें

* class [AvailabilityPeriod](../../availabilityperiod/)
* class [AvailabilityPeriodCollection](../)
* namespace [Aspose.Tasks](../../availabilityperiodcollection/)
* assembly [Aspose.Tasks](../../../)


