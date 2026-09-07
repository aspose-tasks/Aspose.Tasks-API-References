---
title: "ByYearWeekDayRepetition.Month"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ByYearWeekDayRepetition प्रॉपर्टी। वह महीना प्राप्त करता है या सेट करता है, जिस पर कार्य दोहराया जाना चाहिए।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/byyearweekdayrepetition/month/
---
## ByYearWeekDayRepetition.Month property

कार्य को दोहराने वाले महीने को प्राप्त करता है या सेट करता है।

```csharp
public Month Month { get; set; }
```

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

* enum [Month](../../month/)
* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


