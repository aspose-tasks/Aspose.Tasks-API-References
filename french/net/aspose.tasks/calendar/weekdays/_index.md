---
title: "Calendar.WeekDays"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient WeekDaysCollection pour ce calendrier. La collection des jours de la semaine qui définit le calendrier"
type: docs
weight: 120
url: /fr/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Obtient WeekDaysCollection pour ce calendrier. La collection des jours de la semaine qui définit le calendrier.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Exemples

Montre comment définir un nouveau calendrier, y ajouter les jours de la semaine et définir les heures de travail pour les jours.

```csharp
var project = new Project();

// Définir un calendrier
var calendar = project.Calendars.Add("Calendar1");

// Ajouter les jours de travail du lundi au jeudi avec les horaires par défaut
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Définir le vendredi comme jour de travail court
var weekDay = new WeekDay(DayType.Friday);

// Définit le temps de travail. Seule la partie heure de DateTime est importante
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// travail avec le projet...
```

### Voir aussi

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


