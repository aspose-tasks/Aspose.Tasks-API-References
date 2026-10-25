---
title: "एनम RecurrencePattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RecurrencePattern एनम। आवर्ती कार्य के पुनरावृत्ति पैटर्न के प्रकार का प्रतिनिधित्व करता है।"
type: docs
weight: 1690
url: /hi/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

एक आवर्ती कार्य के पुनरावृत्ति पैटर्न के प्रकार का प्रतिनिधित्व करता है।

```csharp
[Flags]
public enum RecurrencePattern
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Daily | `1` | दैनिक पैटर्न। |
| Weekly | `4` | साप्ताहिक पैटर्न। |
| Monthly | `8` | मासिक पैटर्न। |
| Yearly | `10` | वार्षिक पैटर्न। |

## उदाहरण

एक आवर्ती टास्क बनाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


