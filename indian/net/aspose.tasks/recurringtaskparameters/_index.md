---
title: "क्लास RecurringTaskParameters"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RecurringTaskParameters क्लास। एक परियोजना में आवर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट का प्रतिनिधित्व करता है।"
type: docs
weight: 1730
url: /hi/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

प्रोजेक्ट में एक आवर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट को दर्शाता है।

```csharp
public class RecurringTaskParameters
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | `RecurringTaskParameters` क्लास का नया इंस्टेंस प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | आवर्ती कार्य की एक घटना के लिए अवधि प्राप्त करता है या सेट करता है। यह [`Duration`](./duration/) क्लास का इंस्टेंस है। |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि क्या आवर्ती कार्य को तब भी शेड्यूल किया जाए जब कोई संसाधन उपलब्ध न हो। |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | आवर्ती कार्य के पुनरावृत्ति पैटर्न को प्राप्त करता है या सेट करता है। यह [`RecurrencePattern`](./recurrencepattern/) एन्‍युमरेशन के मानों में से एक हो सकता है। |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | आवर्ती कार्य का नाम प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | आवर्ती कार्य के लिए कैलेंडर सेट करें। कैलेंडर परियोजना कैलेंडर संग्रह से चयनित किया जाता है। |

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


