---
title: "Enum Month"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Month enum. Specificeert de maand"
type: docs
weight: 1040
url: /nl/net/aspose.tasks/month/
---
## Month enumeration

Specificeert de maand.

```csharp
public enum Month
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft aan dat de waarde niet gedefinieerd was in het oorspronkelijke projectbestand. |
| January | `0` | Geeft de maand januari aan. |
| February | `1` | Geeft de maand februari aan. |
| March | `2` | Geeft de maand maart aan. |
| April | `3` | Geeft de maand april aan. |
| May | `4` | Geeft de maand mei aan. |
| June | `5` | Geeft de maand juni aan. |
| July | `6` | Geeft de maand juli aan. |
| August | `7` | Geeft de maand augustus aan. |
| September | `8` | Geeft de maand september aan. |
| October | `9` | Geeft de maand oktober aan. |
| November | `10` | Geeft de maand november aan. |
| December | `11` | Geeft de maand december aan. |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe te werken met jaar-dag herhalingen bij het maken van nieuwe terugkerende taken.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


