---
title: "Κλάση AvailabilityPeriod"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.AvailabilityPeriod class. Αντιπροσωπεύει μια περίοδο κατά την οποία ένας πόρος είναι διαθέσιμος"
type: docs
weight: 80
url: /el/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Αντιπροσωπεύει μια περίοδο κατά την οποία ένας πόρος είναι διαθέσιμος.

```csharp
public class AvailabilityPeriod
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Αρχικοποιεί μια νέα παρουσία του `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Αρχικοποιεί μια νέα παρουσία του `AvailabilityPeriod` με το καθορισμένο εύρος ημερομηνιών και τις διαθέσιμες μονάδες. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία κατά την οποία ένας πόρος γίνεται διαθέσιμος για την καθορισμένη περίοδο. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Λαμβάνει ή ορίζει την τελευταία ημερομηνία κατά την οποία ένας πόρος είναι διαθέσιμος για την καθορισμένη περίοδο. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Λαμβάνει ή ορίζει το ποσοστό ενός πόρου που είναι διαθέσιμο κατά τη διάρκεια της καθορισμένης περιόδου. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


