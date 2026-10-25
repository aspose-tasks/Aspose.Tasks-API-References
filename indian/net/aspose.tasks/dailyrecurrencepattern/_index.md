---
title: "क्लास DailyRecurrencePattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.DailyRecurrencePattern क्लास। वह पैरामीटर सेट दर्शाता है जिसका उपयोग प्रोजेक्ट में दैनिक आवर्ती कार्य बनाने के लिए किया जाता है।"
type: docs
weight: 400
url: /hi/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

प्रोजेक्ट में दैनिक पुनरावर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट का प्रतिनिधित्व करता है।

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | `DailyRecurrencePattern` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | आवृत्ति रेंज को प्राप्त करता है या सेट करता है। |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | दैनिक आवृत्ति पैटर्न में पुनरावृत्ति के पैटर्न को प्राप्त करता है या सेट करता है। |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


