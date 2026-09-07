---
title: "WeeklyRepetitionBase.RepetitionInterval"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WeeklyRepetitionBase प्रॉपर्टी। उन हफ्तों की संख्या प्राप्त करता है या सेट करता है जो घटनाओं के बीच अंतराल को दर्शाती है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/weeklyrepetitionbase/repetitioninterval/
---
## WeeklyRepetitionBase.RepetitionInterval property

आवृत्तियों के बीच सप्ताहों में अंतराल को दर्शाने वाले सप्ताहों की संख्या को प्राप्त या सेट करता है।

```csharp
public int RepetitionInterval { get; set; }
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

* class [WeeklyRepetitionBase](../)
* namespace [Aspose.Tasks](../../weeklyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


