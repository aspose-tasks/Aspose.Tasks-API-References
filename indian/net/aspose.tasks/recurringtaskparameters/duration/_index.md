---
title: "RecurringTaskParameters.Duration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RecurringTaskParameters प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो आवर्ती कार्य की एक घटना की अवधि है। Duration क्लास का इंस्टेंस"
type: docs
weight: 20
url: /hi/net/aspose.tasks/recurringtaskparameters/duration/
---
## RecurringTaskParameters.Duration property

मान प्राप्त करता है या सेट करता है जो आवर्ती कार्य की एक घटना की अवधि है। `Duration` क्लास का इंस्टेंस।

```csharp
public Duration Duration { get; set; }
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

* struct [Duration](../../duration/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


