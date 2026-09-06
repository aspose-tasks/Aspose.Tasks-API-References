---
title: "CalendarException.WorkingTimes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CalendarException. Obtient ou définit l'objet WorkingTimeCollection. La collection des temps de travail qui définit le temps travaillé pendant la semaine. Au moins un temps de travail doit être présent et il ne peut pas y en avoir plus de cinq."
type: docs
weight: 160
url: /fr/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Obtient ou définit l'objet WorkingTimeCollection. La collection des temps de travail qui définit le temps travaillé pendant la semaine. Au moins un temps de travail doit être présent, et il ne peut pas y en avoir plus de cinq.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

## Exemples

Montre comment obtenir le temps de travail d'une exception de calendrier.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### Voir aussi

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


