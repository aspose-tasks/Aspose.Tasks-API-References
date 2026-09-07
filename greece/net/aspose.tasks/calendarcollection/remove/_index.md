---
title: "CalendarCollection.Remove"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarCollection μέθοδος. Αφαιρεί το Calendar από το Project CalendarCollection"
type: docs
weight: 60
url: /el/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Αφαιρεί το Calendar από τη συλλογή CalendarCollection του Project.

```csharp
public bool Remove(Calendar item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | Calendar | Το ημερολόγιο προς αφαίρεση. |

### Τιμή Επιστροφής

Εάν αφαιρεθεί επιστρέφει true, αλλιώς επιστρέφει false.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εκτοπίζεται όταν δεν είναι δυνατόν να αφαιρεθεί το ημερολόγιο. |

## Παραδείγματα

Δείχνει πώς να αντικαταστήσετε ένα ημερολόγιο στη συλλογή.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// προσθέστε νέο ημερολόγιο
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


