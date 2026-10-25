---
title: "WeekDay.Clone"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode WeekDay. Retourne une copie profonde du jour de la semaine"
type: docs
weight: 80
url: /fr/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

Renvoie une copie profonde du jour de la semaine.

```csharp
public WeekDay Clone()
```

### Valeur de retour

Retourne la copie profonde du jour de la semaine.

## Exemples

Montre comment cloner un jour de la semaine.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// créer une copie profonde d'un jour de la semaine
var weekDay2 = weekDay1.Clone();

// l'égalité des calendriers est vérifiée par rapport aux propriétés du jour de la semaine :
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### Voir aussi

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


