---
title: "Énumération Month"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Month. Spécifie le mois"
type: docs
weight: 1040
url: /fr/net/aspose.tasks/month/
---
## Month enumeration

Spécifie le mois.

```csharp
public enum Month
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique que la valeur n'était pas définie dans le fichier de projet original. |
| January | `0` | Indique le mois de janvier. |
| February | `1` | Indique le mois de février. |
| March | `2` | Indique le mois de mars. |
| April | `3` | Indique le mois d'avril. |
| May | `4` | Indique le mois de mai. |
| June | `5` | Indique le mois de juin. |
| July | `6` | Indique le mois de juillet. |
| August | `7` | Indique le mois d'août. |
| September | `8` | Indique le mois de septembre. |
| October | `9` | Indique le mois d'octobre. |
| November | `10` | Indique le mois de novembre. |
| December | `11` | Indique le mois de décembre. |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


