---
title: "CalendarCollection.GetByName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος CalendarCollection. Επιστρέφει ένα ημερολόγιο με το καθορισμένο όνομα"
type: docs
weight: 30
url: /el/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Επιστρέφει ένα ημερολόγιο με το καθορισμένο όνομα.

```csharp
public Calendar GetByName(string name)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα ενός ημερολογίου. |

### Τιμή Επιστροφής

Εάν βρεθεί, επιστρέφει το ημερολόγιο με το καθορισμένο όνομα, διαφορετικά επιστρέφει null.

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


