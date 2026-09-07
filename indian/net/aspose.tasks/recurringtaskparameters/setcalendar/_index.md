---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RecurringTaskParameters मेथड। आवर्ती कार्य के लिए कैलेंडर सेट करता है। कैलेंडर प्रोजेक्ट कैलेंडर संग्रह से चयनित किया जाता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

आवर्ती कार्य के लिए कैलेंडर सेट करें। कैलेंडर परियोजना कैलेंडर संग्रह से चयनित किया जाता है।

```csharp
public void SetCalendar(Project project, string calendarName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | कैलेंडर संग्रह वाला प्रोजेक्ट। |
| calendarName | स्ट्रिंग | कैलेंडर का नाम। |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


