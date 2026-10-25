---
title: "CalendarCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarCollection μέθοδος. Επιστρέφει έναν ενομετρητή για αυτή τη συλλογή"
type: docs
weight: 50
url: /el/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Τιμή Επιστροφής

έναν απαριθμητή για αυτή τη συλλογή.

## Παραδείγματα

Δείχνει πώς να προσθέσετε νέα ημερολόγια.

```csharp
var project = new Project();

// Νέα ημερολόγια μπορούν να προστεθούν στη συλλογή ημερολογίων ενός έργου χρησιμοποιώντας τις υπερφορτώσεις Add της συλλογής.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


