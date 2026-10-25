---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier"
type: docs
weight: 160
url: /fr/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | Date de début. |
| work | Duration | Durée du travail. |

### Valeur de retour

Date de fin.

## Exemples

Montre comment calculer une date de fin à partir de la date de début et du travail en utilisant une instance de calendrier.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calculer la date de fin en utilisant un calendrier standard
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Voir aussi

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | Date de début. |
| work | TimeSpan | Durée du travail. |

### Valeur de retour

Date de fin.

## Exemples

Montre comment calculer une date de fin à partir de la date de début et du travail (en tant que durée) en utilisant une instance de calendrier.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calculer la date de fin en utilisant un calendrier standard
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


