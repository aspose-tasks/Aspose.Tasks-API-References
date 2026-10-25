---
title: "Resource.AvailabilityPeriods"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी। AvailabilityPeriodCollection क्लास का एक उदाहरण प्राप्त करता है। वह अवधि संग्रह जिसमें एक संसाधन उपलब्ध रहता है।"
type: docs
weight: 130
url: /hi/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

[`AvailabilityPeriodCollection`](../../availabilityperiodcollection/) क्लास का एक उदाहरण प्राप्त करता है। वह अवधि संग्रह जिसमें एक संसाधन उपलब्ध रहता है।

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## उदाहरण

एक संसाधन के लिए उपलब्धता अवधि जोड़ने का तरीका दर्शाता है।

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

var availabilityPeriod = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 1, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 1, 17, 0, 0),
    AvailableUnits = 2d
};
resource.AvailabilityPeriods.Add(availabilityPeriod);

var availabilityPeriod2 = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 2, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 2, 17, 0, 0),
    AvailableUnits = 3d
};
resource.AvailabilityPeriods.Add(availabilityPeriod2);
```

### संबंधित देखें

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


