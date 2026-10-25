---
title: "CalendarCollection.Count"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarCollection ιδιότητα. Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο CalendarCollection"
type: docs
weight: 10
url: /el/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο [`CalendarCollection`](../).

```csharp
public int Count { get; }
```

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

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


