---
title: "Classe CalendarCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "classe Aspose.Tasks.CalendarCollection. Représente une collection d'objets Calendar"
type: docs
weight: 240
url: /fr/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Représente une collection d'objets [`Calendar`](../calendar/).

```csharp
public class CalendarCollection : IList<Calendar>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Obtient le nombre d'objets contenus dans cet objet `CalendarCollection`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Ajoute un nouveau calendrier de base à cet objet CalendarCollection et renvoie le calendrier ajouté. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Ajoute un nouveau calendrier avec le calendrier de base spécifié à cet objet CalendarCollection et renvoie le calendrier ajouté. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Renvoie un calendrier avec le nom spécifié. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Renvoie un calendrier avec l'UID spécifié. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Supprime Calendar du CalendarCollection du projet. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Convertit l'objet CalendarCollection en une liste d'objets [`Calendar`](../calendar/). |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


