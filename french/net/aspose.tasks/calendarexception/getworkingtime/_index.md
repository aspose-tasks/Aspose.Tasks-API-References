---
title: "CalendarException.GetWorkingTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CalendarException. Retourne le temps de travail pour une exception de calendrier."
type: docs
weight: 200
url: /fr/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Renvoie le temps de travail pour une exception de calendrier.

```csharp
public TimeSpan GetWorkingTime()
```

### Valeur de retour

Retourne le temps de travail pour cette exception de calendrier.

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


