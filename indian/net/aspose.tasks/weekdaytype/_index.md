---
title: "Enum WeekdayType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WeekdayType enum. प्रोजेक्ट के RecurringTaskInfo क्लास की इंस्टेंस में एक सप्ताह का दिन दर्शाता है"
type: docs
weight: 3570
url: /hi/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

एक प्रोजेक्ट के सप्ताह के दिन को [`RecurringTaskInfo`](../recurringtaskinfo/) क्लास की इंस्टेंस में दर्शाता है।

```csharp
[Flags]
public enum WeekdayType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `0` | None सप्ताह के दिन प्रकार को दर्शाता है। |
| Sunday | `1` | Sunday सप्ताह के दिन प्रकार को दर्शाता है। |
| Monday | `2` | Monday सप्ताह के दिन प्रकार को दर्शाता है। |
| Tuesday | `4` | Tuesday सप्ताह के दिन प्रकार को दर्शाता है। |
| Wednesday | `8` | Wednesday सप्ताह के दिन प्रकार को दर्शाता है। |
| Thursday | `10` | Thursday सप्ताह के दिन प्रकार को दर्शाता है। |
| Friday | `20` | Friday सप्ताह के दिन प्रकार को दर्शाता है। |
| Saturday | `40` | Saturday सप्ताह के दिन प्रकार को दर्शाता है। |

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


