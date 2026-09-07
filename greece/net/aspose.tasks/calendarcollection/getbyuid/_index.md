---
title: "CalendarCollection.GetByUid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarCollection μέθοδος. Επιστρέφει ένα ημερολόγιο με το καθορισμένο UID"
type: docs
weight: 40
url: /el/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Επιστρέφει ένα ημερολόγιο με το καθορισμένο UID.

```csharp
public Calendar GetByUid(int uid)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | Int32 | UID ενός ημερολογίου. |

### Τιμή Επιστροφής

Ημερολόγιο με καθορισμένο UID.

## Παραδείγματα

Δείχνει πώς να λαμβάνετε ημερολόγια κατά όνομα ή κατά αναγνωριστικό.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


