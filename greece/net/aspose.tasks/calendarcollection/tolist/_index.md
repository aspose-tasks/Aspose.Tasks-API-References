---
title: "CalendarCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarCollection μέθοδος. Μετατρέπει το αντικείμενο CalendarCollection σε λίστα αντικειμένων Calendar"
type: docs
weight: 70
url: /el/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Μετατρέπει το αντικείμενο CalendarCollection σε λίστα αντικειμένων [`Calendar`](../../calendar/).

```csharp
public List<Calendar> ToList()
```

### Τιμή Επιστροφής

Λίστα αντικειμένων [`Calendar`](../../calendar/).

## Παραδείγματα

Δείχνει πώς να διασχίσετε τη συλλογή ημερολογίων.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


