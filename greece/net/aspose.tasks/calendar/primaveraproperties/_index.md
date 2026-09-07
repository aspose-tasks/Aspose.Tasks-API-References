---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες Primaveraspecific για ένα ημερολόγιο που διαβάζεται από μορφές Primavera"
type: docs
weight: 100
url: /el/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες ειδικές για Primavera για ένα ημερολόγιο που διαβάζεται από μορφές Primavera.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera και να εξετάσετε τις Primavera-specific ιδιότητες του ημερολογίου.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Επιστρέφει έργο με ειδικό UID
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Δείτε επίσης

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


