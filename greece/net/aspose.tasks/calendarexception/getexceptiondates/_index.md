---
title: "CalendarException.GetExceptionDates"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος CalendarException. Επιστρέφει ημερομηνίες στις οποίες η εξαίρεση ημερολογίου είναι εφαρμόσιμη"
type: docs
weight: 190
url: /el/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Επιστρέφει τις ημερομηνίες στις οποίες η εξαίρεση του ημερολογίου είναι εφαρμόσιμη.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Τιμή Επιστροφής

Επιστρέφει μια συλλογή ημερομηνιών εξαίρεσης για τις οποίες η εξαίρεση ημερολογίου είναι εφαρμόσιμη.

## Παραδείγματα

Δείχνει πώς να ληφθούν οι ημερομηνίες για τις οποίες μια συγκεκριμένη εξαίρεση ημερολογίου είναι ενεργή.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### Δείτε επίσης

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


