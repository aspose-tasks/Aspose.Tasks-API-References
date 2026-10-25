---
title: "क्लास EndAfterRecurrenceRange"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.EndAfterRecurrenceRange क्लास। आवर्ती कार्य की पुनरावृत्ति सीमा को दर्शाता है जो घटना संख्या द्वारा सीमित है"
type: docs
weight: 500
url: /hi/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

पुनरावर्ती कार्य की पुनरावृत्ति सीमा का प्रतिनिधित्व करता है जो घटना संख्या द्वारा सीमित है।

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | `EndAfterRecurrenceRange` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | आवर्ती कार्य की पुनरावृत्ति सीमा को सीमित करने वाली घटनाओं की संख्या प्राप्त करता है या सेट करता है। |
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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


