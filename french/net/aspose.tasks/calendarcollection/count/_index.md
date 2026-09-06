---
title: "CalendarCollection.Count"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CalendarCollection. Obtient le nombre d'objets contenus dans cet objet CalendarCollection"
type: docs
weight: 10
url: /fr/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Obtient le nombre d'objets contenus dans cet objet [`CalendarCollection`](../).

```csharp
public int Count { get; }
```

## Exemples

Montre comment itérer sur la collection de calendriers.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Voir aussi

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


