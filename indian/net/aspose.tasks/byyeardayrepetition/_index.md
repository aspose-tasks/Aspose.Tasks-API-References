---
title: "क्लास ByYearDayRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ByYearDayRepetition क्लास। एक पैटर्न का प्रतिनिधित्व करता है जो महीने में किसी दिन की निरपेक्ष स्थिति पर आधारित है।"
type: docs
weight: 190
url: /hi/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

एक पैटर्न का प्रतिनिधित्व करता है जो महीने में किसी दिन की निरपेक्ष स्थिति पर आधारित है।

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | `ByYearDayRepetition` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | कार्य को पुनरावर्ती करने के लिए महीने में दिन की स्थिति प्राप्त करता है या सेट करता है। |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | कार्य को दोहराने वाले महीने को प्राप्त करता है या सेट करता है। |

## उदाहरण

नए पुनरावर्ती कार्य बनाते समय वर्ष-दिन दोहराव के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


