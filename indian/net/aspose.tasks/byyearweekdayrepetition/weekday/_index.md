---
title: "ByYearWeekDayRepetition.WeekDay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ByYearWeekDayRepetition प्रॉपर्टी। वह सप्ताह के दिन का प्रकार प्राप्त करता है या सेट करता है, जिस पर कार्य दोहराया जाना चाहिए।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/byyearweekdayrepetition/weekday/
---
## ByYearWeekDayRepetition.WeekDay property

कार्य को आवर्ती बनाने के लिए जिस सप्ताह के दिन का प्रकार प्राप्त या सेट किया जाता है।

```csharp
public DayOfWeek WeekDay { get; set; }
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

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


