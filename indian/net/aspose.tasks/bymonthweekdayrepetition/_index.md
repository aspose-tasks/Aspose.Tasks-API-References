---
title: "`ByMonthWeekDayRepetition` वर्ग"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "`Aspose.Tasks.ByMonthWeekDayRepetition` वर्ग। यह एक पैटर्न का प्रतिनिधित्व करता है जो महीने में सप्ताह के दिन की स्थिति पर आधारित है।"
type: docs
weight: 180
url: /hi/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

एक पैटर्न का प्रतिनिधित्व करता है जो महीने में सप्ताह के दिन की स्थिति पर आधारित है।

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | `ByMonthWeekDayRepetition` वर्ग का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | कार्य को दोहराने के लिए महीने में सप्ताह के दिन की स्थिति को प्राप्त करता है या सेट करता है। |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | घटनाओं के बीच महीनों में अंतराल दर्शाने वाले महीने की संख्या को प्राप्त करता है या सेट करता है। |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | कार्य को दोहराने के लिए सप्ताह के दिन के प्रकार को प्राप्त करता है या सेट करता है। |

## उदाहरण

नए दोहराव वाले कार्य बनाते समय महीने के सप्ताह के दिन की पुनरावृत्तियों के साथ कैसे काम करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


