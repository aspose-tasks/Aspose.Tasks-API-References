---
title: "क्लास WeeklyRepetitionBase"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WeeklyRepetitionBase क्लास. साप्ताहिक आवृत्ति पैटर्न में पुनरावृत्तियों के लिए एक बेस क्लास का प्रतिनिधित्व करती है।"
type: docs
weight: 3600
url: /hi/net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

साप्ताहिक आवर्ती पैटर्न में दोहराव के लिए बेस क्लास दर्शाता है।

```csharp
public abstract class WeeklyRepetitionBase
```

## गुण

| नाम | विवरण |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | आवृत्तियों के बीच सप्ताहों में अंतराल को दर्शाने वाले सप्ताहों की संख्या को प्राप्त या सेट करता है। |

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


