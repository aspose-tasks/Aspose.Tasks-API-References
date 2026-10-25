---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Retourne la date de début basée sur la date de fin et la durée spécifiées"
type: docs
weight: 200
url: /fr/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Renvoie la date de début basée sur la date de fin et la durée spécifiées.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fin | DateTime | La date de fin spécifiée. |
| duration | Duration | La durée spécifiée. |

### Valeur de retour

Date de début calculée.

## Exemples

Montre comment obtenir une date de début à partir de la date de fin et de la durée.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenir la date de début à partir de la date de fin et d'une durée
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// Le 8 avril 2020 09:00 sera imprimé
Console.WriteLine(startDate);
```

### Voir aussi

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Renvoie la date de début basée sur la date de fin et la durée spécifiées.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fin | DateTime | La date de fin spécifiée. |
| duration | TimeSpan | La durée spécifiée. |

### Valeur de retour

Date de début calculée.

## Exemples

Montre comment obtenir une date de début à partir de la date de fin et de la durée (en tant qu'intervalle de temps).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenir la date de début à partir de la date de fin et d'une durée
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// Le 8 avril 2020 09:00 sera imprimé
Console.WriteLine(startDate);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


