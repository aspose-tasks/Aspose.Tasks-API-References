---
title: "क्लास RecurrenceRangeBase"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RecurrenceRangeBase क्लास। आवर्ती कार्य की पुनरावृत्ति सीमा का प्रतिनिधित्व करता है।"
type: docs
weight: 1710
url: /hi/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

आवर्ती कार्य की आवर्ती सीमा को दर्शाता है।

```csharp
public abstract class RecurrenceRangeBase
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | आवर्ती कार्य की पुनरावृत्ति सीमा की प्रारंभ तिथि प्राप्त करता है या सेट करता है। |

## उदाहरण

आवर्ती कार्य बनाते समय दैनिक कार्य पुनरावृत्ति पैटर्न की पुनरावृत्तियों के साथ कैसे काम किया जाए, यह दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// परियोजना के साथ आगे काम करें...
// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


