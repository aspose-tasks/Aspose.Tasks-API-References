---
title: "EndAfterRecurrenceRange.EndAfterRecurrenceRange"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "EndAfterRecurrenceRange कंस्ट्रक्टर। EndAfterRecurrenceRange क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/endafterrecurrencerange/endafterrecurrencerange/
---
## EndAfterRecurrenceRange constructor

एक नया इंस्टेंस इनिशियलाइज़ करता है [`EndAfterRecurrenceRange`](../) क्लास का।

```csharp
public EndAfterRecurrenceRange()
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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


