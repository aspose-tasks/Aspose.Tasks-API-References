---
title: "EndByRecurrenceRange.Finish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "EndByRecurrenceRange प्रॉपर्टी। आवर्ती कार्य की पुनरावृत्ति सीमा को सीमित करने वाली तिथि को प्राप्त करता है और सेट करता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/endbyrecurrencerange/finish/
---
## EndByRecurrenceRange.Finish property

आवर्ती कार्य की पुनरावृत्ति सीमा को सीमित करने वाली तिथि को प्राप्त करता है या सेट करता है।

```csharp
public DateTime Finish { get; set; }
```

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

* class [EndByRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endbyrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


