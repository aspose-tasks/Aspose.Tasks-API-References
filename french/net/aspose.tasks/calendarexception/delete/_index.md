---
title: "CalendarException.Delete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "CalendarException méthode. Supprime l'instance Exception de l'objet calendrier parent CalendarExceptionCollection."
type: docs
weight: 180
url: /fr/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Supprime l'instance Exception de l'objet calendrier parent CalendarExceptionCollection.

```csharp
public void Delete()
```

## Exemples

Montre comment supprimer une exception de calendrier.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// supprimez l'exception
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### Voir aussi

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


