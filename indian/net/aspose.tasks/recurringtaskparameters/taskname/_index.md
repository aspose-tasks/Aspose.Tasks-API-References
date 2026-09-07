---
title: "RecurringTaskParameters.TaskName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RecurringTaskParameters प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो आवर्ती कार्य का नाम है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/recurringtaskparameters/taskname/
---
## RecurringTaskParameters.TaskName property

आवर्ती कार्य का नाम प्राप्त करता है या सेट करता है।

```csharp
public string TaskName { get; set; }
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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


