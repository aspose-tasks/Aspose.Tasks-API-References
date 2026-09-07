---
title: "क्लास WeeklyRecurrencePattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WeeklyRecurrencePattern क्लास। पैरामीटर्स का सेट दर्शाता है जिसका उपयोग प्रोजेक्ट में साप्ताहिक आवर्ती टास्क बनाने के लिए किया जाता है।"
type: docs
weight: 3580
url: /hi/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

प्रोजेक्ट में साप्ताहिक आवर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट को दर्शाता है।

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | `WeeklyRecurrencePattern` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | आवृत्ति रेंज को प्राप्त करता है या सेट करता है। |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | आवर्ती पुनरावृत्ति पैटर्न को प्राप्त करता है या सेट करता है। |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


