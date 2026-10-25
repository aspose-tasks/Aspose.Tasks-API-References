---
title: "Calendar.IsBaselineCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι ημερολόγιο βάσης"
type: docs
weight: 80
url: /el/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι ημερολόγιο βάσης.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ελέγξετε εάν ένα ημερολόγιο είναι ημερολόγιο βάσης ή όχι.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


