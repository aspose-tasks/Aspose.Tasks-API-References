---
title: "CalendarCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CalendarCollection. Retourne un énumérateur pour cette collection."
type: docs
weight: 50
url: /fr/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Renvoie un énumérateur pour cette collection.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Valeur de retour

un énumérateur pour cette collection.

## Exemples

Montre comment ajouter de nouveaux calendriers.

```csharp
var project = new Project();

// De nouveaux calendriers peuvent être ajoutés à la collection de calendriers d'un projet en utilisant les surcharges de la méthode Add de la collection.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Voir aussi

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


