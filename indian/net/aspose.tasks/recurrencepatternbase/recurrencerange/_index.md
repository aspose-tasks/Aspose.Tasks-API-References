---
title: "RecurrencePatternBase.RecurrenceRange"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RecurrencePatternBase प्रॉपर्टी। आवर्ती रेंज को प्राप्त या सेट करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/recurrencepatternbase/recurrencerange/
---
## RecurrencePatternBase.RecurrenceRange property

आवृत्ति रेंज को प्राप्त करता है या सेट करता है।

```csharp
public RecurrenceRangeBase RecurrenceRange { get; set; }
```

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

* class [RecurrenceRangeBase](../../recurrencerangebase/)
* class [RecurrencePatternBase](../)
* namespace [Aspose.Tasks](../../recurrencepatternbase/)
* assembly [Aspose.Tasks](../../../)


