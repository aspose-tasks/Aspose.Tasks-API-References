---
title: "Énumération BookingType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.BookingType. Spécifie le type de réservation d'une ressource"
type: docs
weight: 150
url: /fr/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Spécifie le type de réservation d’une ressource.

```csharp
public enum BookingType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique que la valeur n'était pas définie dans le fichier de projet original. |
| Committed | `0` | Indique le type de réservation engagé. |
| Proposed | `1` | Indique le type de réservation proposé. |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment lire/écrire la propriété Asn.BookingType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


