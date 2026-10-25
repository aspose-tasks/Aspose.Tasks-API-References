---
title: "क्लास EndByRecurrenceRange"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.EndByRecurrenceRange क्लास। आवर्ती कार्य की पुनरावृत्ति सीमा का प्रतिनिधित्व करता है जो समाप्ति दिन द्वारा सीमित है।"
type: docs
weight: 510
url: /hi/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

पुनरावर्ती कार्य की पुनरावृत्ति सीमा का प्रतिनिधित्व करता है जो समाप्ति दिन द्वारा सीमित है।

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | `EndByRecurrenceRange` क्लास का एक नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | आवर्ती कार्य की पुनरावृत्ति सीमा को सीमित करने वाली तिथि को प्राप्त करता है या सेट करता है। |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | आवर्ती कार्य की पुनरावृत्ति सीमा की प्रारंभ तिथि प्राप्त करता है या सेट करता है। |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


