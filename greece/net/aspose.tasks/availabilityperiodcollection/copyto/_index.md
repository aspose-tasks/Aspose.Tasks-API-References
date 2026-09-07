---
title: "AvailabilityPeriodCollection.CopyTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "AvailabilityPeriodCollection μέθοδος. Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα ξεκινώντας από τον καθορισμένο δείκτη του πίνακα"
type: docs
weight: 80
url: /el/net/aspose.tasks/availabilityperiodcollection/copyto/
---
## AvailabilityPeriodCollection.CopyTo method

Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα.

```csharp
public void CopyTo(AvailabilityPeriod[] array, int arrayIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | AvailabilityPeriod[] | ο καθορισμένος μονοδιάστατος πίνακας για αντιγραφή των στοιχείων σε αυτόν |
| arrayIndex | Int32 | ο μηδενικός δείκτης του καθορισμένου πίνακα στον οποίο αρχίζει η αντιγραφή. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη συλλογή περιόδων διαθεσιμότητας του πόρου.

```csharp
public void WorkWithAvailabilityPeriodCollection()
{
    var project = new Project(DataDir + "UpdateResourceData.mpp");
    var resource = project.Resources.GetById(1);

    resource.AvailabilityPeriods.Clear();

    // Προσθέστε περιόδους διαθεσιμότητας (έτη 2012 και 2014) στο νέο πόρο
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

    // ενημερώστε τις διαθέσιμες μονάδες για την περίοδο του έτους 2014
    otherResource.AvailabilityPeriods[otherResource.AvailabilityPeriods.Count - 2].AvailableUnits = 0.90;

    // αφαιρέστε την περίοδο του 2013
    otherResource.AvailabilityPeriods.Remove(period2013);

    // αφαιρέστε την περίοδο του 2011
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

### Δείτε επίσης

* class [AvailabilityPeriod](../../availabilityperiod/)
* class [AvailabilityPeriodCollection](../)
* namespace [Aspose.Tasks](../../availabilityperiodcollection/)
* assembly [Aspose.Tasks](../../../)


