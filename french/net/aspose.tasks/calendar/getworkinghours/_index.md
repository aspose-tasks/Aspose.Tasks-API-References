---
title: "Calendar.GetWorkingHours"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Retourne WorkUnit, Start, Finish et Duration des heures de travail pour l'intervalle de dates et heures spécifié"
type: docs
weight: 220
url: /fr/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de date et d'heure spécifié.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | Date de début de l'intervalle. |
| fin | DateTime | Date de fin de l'intervalle. |

### Valeur de retour

Instance de la classe [`WorkUnit`](../../workunit/) contenant le Début, la Fin et la Durée des heures de travail.

## Exemples

Montre comment obtenir les heures de travail pour des dates spécifiques.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenez les heures de travail pour une date spécifique
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16 heures seront affichées
Console.WriteLine(workUnit.WorkingHours);
```

### Voir aussi

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Renvoie le nombre d'heures de travail à la date spécifiée.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dt | DateTime | La date pour laquelle obtenir les heures de travail. |

### Valeur de retour

Heures de travail à la date spécifiée.

## Exemples

Montre comment obtenir les heures de travail pour une date spécifique.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenez les heures de travail pour une date spécifique
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 8 heures seront affichées
Console.WriteLine(workingHours.Hours);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


