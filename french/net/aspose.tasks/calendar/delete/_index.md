---
title: "Calendar.Delete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Supprime le calendrier du projet"
type: docs
weight: 140
url: /fr/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Supprime le calendrier du projet.

```csharp
public void Delete()
```

## Exemples

Montre comment supprimer un calendrier d'un projet.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// obtenir le calendrier par son nom
var calendar = project.Calendars.GetByName("Broken Calendar");

// supprimer le calendrier
calendar.Delete();
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


