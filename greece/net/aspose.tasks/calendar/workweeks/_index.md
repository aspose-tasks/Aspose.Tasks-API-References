---
title: "Calendar.WorkWeeks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει το αντικείμενο WorkWeekCollections. Η συλλογή των εβδομάδων εργασίας που σχετίζονται με το ημερολόγιο"
type: docs
weight: 130
url: /el/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Λαμβάνει το αντικείμενο WorkWeekCollections. Η συλλογή των εβδομάδων εργασίας που σχετίζονται με το ημερολόγιο.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε πληροφορίες εβδομάδας εργασίας.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Εμφάνιση ονόματος εβδομάδας εργασίας, από και έως ημερομηνίες
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Αυτά τα δεδομένα αφορούν το κουμπί "Λεπτομέρειες". Μπορείτε να ορίσετε ειδικούς χρόνους εργασίας για συγκεκριμένη ημέρα της εβδομάδας ή ακόμη και να την κάνετε μη εργάσιμη.
    foreach (var day in workWeek.WeekDays)
    {
        // Μπορείτε περαιτέρω να διασχίσετε τους χρόνους εργασίας και να τους εμφανίσετε.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### Δείτε επίσης

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


