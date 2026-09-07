---
title: "क्लास MonthlyRecurrencePattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.MonthlyRecurrencePattern क्लास। उन पैरामीटरों के सेट का प्रतिनिधित्व करता है जो प्रोजेक्ट में मासिक आवर्ती कार्य बनाने के लिए उपयोग किए जाते हैं।"
type: docs
weight: 1080
url: /hi/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

प्रोजेक्ट में मासिक आवर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट का प्रतिनिधित्व करता है।

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | `MonthlyRecurrencePattern` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | आवृत्ति रेंज को प्राप्त करता है या सेट करता है। |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | आवर्ती पुनरावृत्ति पैटर्न को प्राप्त करता है या सेट करता है। |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


