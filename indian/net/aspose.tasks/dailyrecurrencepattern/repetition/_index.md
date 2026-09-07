---
title: "DailyRecurrencePattern.Repetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "DailyRecurrencePattern प्रॉपर्टी। प्राप्त करता है या सेट करता है दैनिक आवृत्ति पैटर्न में पुनरावृत्ति का पैटर्न"
type: docs
weight: 20
url: /hi/net/aspose.tasks/dailyrecurrencepattern/repetition/
---
## DailyRecurrencePattern.Repetition property

दैनिक आवृत्ति पैटर्न में पुनरावृत्ति के पैटर्न को प्राप्त करता है या सेट करता है।

```csharp
public DailyRepetitionBase Repetition { get; set; }
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

* class [DailyRepetitionBase](../../dailyrepetitionbase/)
* class [DailyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../dailyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


