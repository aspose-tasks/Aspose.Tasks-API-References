---
title: "Class ByMonthDayRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ByMonthDayRepetition class. एक पैटर्न का प्रतिनिधित्व करता है जो महीने में किसी दिन की निरपेक्ष स्थिति पर आधारित है।"
type: docs
weight: 170
url: /hi/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

एक पैटर्न का प्रतिनिधित्व करता है जो महीने में किसी दिन की निरपेक्ष स्थिति पर आधारित है।

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() |  `ByMonthDayRepetition` class का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | महीने में उस दिन की स्थिति प्राप्त करता है या सेट करता है जिस पर कार्य को दोहराया जाना चाहिए। |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | घटनाओं के बीच महीनों में अंतराल दर्शाने वाले महीने की संख्या को प्राप्त करता है या सेट करता है। |

## उदाहरण

नए आवर्ती कार्य बनाते समय महीने के दिन दोहराव के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


