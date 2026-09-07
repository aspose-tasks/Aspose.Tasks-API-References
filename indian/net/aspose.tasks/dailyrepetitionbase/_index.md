---
title: "क्लास DailyRepetitionBase"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.DailyRepetitionBase क्लास। दैनिक आवृत्ति पैटर्न में पुनरावृत्तियों के लिए एक बेस क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 410
url: /hi/net/aspose.tasks/dailyrepetitionbase/
---
## DailyRepetitionBase class

दैनिक पुनरावृत्ति पैटर्न में दोहराव के लिए एक बेस क्लास का प्रतिनिधित्व करता है।

```csharp
public abstract class DailyRepetitionBase
```

## गुण

| नाम | विवरण |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | घटनाओं के बीच दिनों में अंतराल को दर्शाने वाले दिनों की संख्या को प्राप्त करता है या सेट करता है। |

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


