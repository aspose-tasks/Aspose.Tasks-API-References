---
title: "ByYearDayRepetition.Month"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ByYearDayRepetition. Obtient ou définit le mois pendant lequel la tâche doit être récurrente"
type: docs
weight: 30
url: /fr/net/aspose.tasks/byyeardayrepetition/month/
---
## ByYearDayRepetition.Month property

Obtient ou définit le mois pendant lequel la tâche doit être récurrente.

```csharp
public Month Month { get; set; }
```

## Exemples

Montre comment travailler avec les répétitions de jour de l'année lors de la création de nouvelles tâches récurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* enum [Month](../../month/)
* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


