---
title: "CalendarCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CalendarCollection. Convertit l'objet CalendarCollection en une liste d'objets Calendar."
type: docs
weight: 70
url: /fr/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Convertit l'objet CalendarCollection en une liste d'objets [`Calendar`](../../calendar/).

```csharp
public List<Calendar> ToList()
```

### Valeur de retour

Liste d'objets [`Calendar`](../../calendar/).

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


