---
title: "क्लास MonthlyRepetitionBase"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.MonthlyRepetitionBase क्लास। मासिक दिन स्थिति के लिए एक बेस पैटर्न का प्रतिनिधित्व करता है"
type: docs
weight: 1090
url: /hi/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

मासिक दिन स्थिति के लिए एक बेस पैटर्न का प्रतिनिधित्व करता है।

```csharp
public abstract class MonthlyRepetitionBase
```

## गुण

| नाम | विवरण |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | घटनाओं के बीच महीनों में अंतराल दर्शाने वाले महीने की संख्या को प्राप्त करता है या सेट करता है। |

## उदाहरण

दिखाता है कि आवर्ती कार्य बनाते समय मासिक पुनरावृत्ति पैटर्न दोहराव के साथ कैसे काम किया जाए।

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


