---
title: "ByMonthWeekDayRepetition.ByMonthWeekDayRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ByMonthWeekDayRepetition कन्स्ट्रक्टर। ByMonthWeekDayRepetition क्लास का नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/bymonthweekdayrepetition/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition constructor

[`ByMonthWeekDayRepetition`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ByMonthWeekDayRepetition()
```

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

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


