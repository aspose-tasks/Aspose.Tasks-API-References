---
title: "Calendar.Exceptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει το αντικείμενο CalendarExceptionCollection. Η συλλογή των εξαιρέσεων που σχετίζονται με το ημερολόγιο."
type: docs
weight: 50
url: /el/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Λαμβάνει το αντικείμενο CalendarExceptionCollection. Η συλλογή των εξαιρέσεων που σχετίζονται με το ημερολόγιο.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Παραδείγματα

Δείχνει πώς να ανακτήσετε πληροφορίες σχετικά με τις εξαιρέσεις του ημερολογίου.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Επανάληψη μέσω ημερολογίων
foreach (var calendar in project.Calendars)
{
    // Πρόσβαση σε εξαιρέσεις ημερολογίου
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### Δείτε επίσης

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


