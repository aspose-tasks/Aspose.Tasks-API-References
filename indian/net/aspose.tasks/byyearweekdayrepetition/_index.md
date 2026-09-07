---
title: "क्लास ByYearWeekDayRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ByYearWeekDayRepetition क्लास। यह एक पैटर्न का प्रतिनिधित्व करता है जो महीने में सप्ताह के दिन की स्थिति पर आधारित है।"
type: docs
weight: 200
url: /hi/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

एक पैटर्न का प्रतिनिधित्व करता है जो महीने में सप्ताह के दिन की स्थिति पर आधारित है।

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | `ByYearWeekDayRepetition` क्लास का नया उदाहरण इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | कार्य को दोहराने वाले महीने को प्राप्त करता है या सेट करता है। |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | कार्य को दोहराने वाले महीने के सप्ताह में दिन की स्थिति को प्राप्त करता है या सेट करता है। |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | कार्य को आवर्ती बनाने के लिए जिस सप्ताह के दिन का प्रकार प्राप्त या सेट किया जाता है। |

## उदाहरण

नए आवर्ती कार्य बनाते समय वर्ष के सप्ताह के दिन की पुनरावृत्तियों के साथ कैसे काम किया जाए, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


