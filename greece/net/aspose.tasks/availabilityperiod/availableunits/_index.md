---
title: "AvailabilityPeriod.AvailableUnits"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα AvailabilityPeriod. Λαμβάνει ή ορίζει το ποσοστό ενός πόρου που είναι διαθέσιμο κατά τη διάρκεια της καθορισμένης περιόδου"
type: docs
weight: 40
url: /el/net/aspose.tasks/availabilityperiod/availableunits/
---
## AvailabilityPeriod.AvailableUnits property

Λαμβάνει ή ορίζει το ποσοστό ενός πόρου που είναι διαθέσιμο κατά τη διάρκεια της καθορισμένης περιόδου.

```csharp
public double AvailableUnits { get; set; }
```

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε περιόδους διαθεσιμότητας για έναν πόρο.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Προσθέστε περιόδους διαθεσιμότητας σε νέο πόρο
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

### Δείτε επίσης

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


