---
title: "Calendar.PrimaveraProperties"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient un objet contenant les propriétés spécifiques à Primavera pour un calendrier lu à partir des formats Primavera."
type: docs
weight: 100
url: /fr/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Obtient un objet contenant les propriétés spécifiques à Primavera pour un calendrier lu à partir des formats Primavera.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Exemples

Montre comment lire un projet à partir d'un fichier Primavera et examiner les propriétés spécifiques à Primavera du calendrier.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Renvoie le projet avec un UID spécial
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Voir aussi

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


