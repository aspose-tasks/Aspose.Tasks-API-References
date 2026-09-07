---
title: "क्लास WeeklyRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WeeklyRepetition क्लास। एक पैटर्न का प्रतिनिधित्व करता है जो सप्ताह के दिनों पर आधारित है।"
type: docs
weight: 3590
url: /hi/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

सप्ताह के दिनों पर आधारित पैटर्न दर्शाता है।

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | `WeeklyRepetition` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | आवृत्तियों के बीच सप्ताहों में अंतराल को दर्शाने वाले सप्ताहों की संख्या को प्राप्त या सेट करता है। |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | सप्ताह के दिनों का प्रकार प्राप्त करता है या सेट करता है। |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


