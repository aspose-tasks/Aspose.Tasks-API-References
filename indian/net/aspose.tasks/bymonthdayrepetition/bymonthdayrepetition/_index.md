---
title: "ByMonthDayRepetition.ByMonthDayRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ByMonthDayRepetition कंस्ट्रक्टर। ByMonthDayRepetition क्लास का नया उदाहरण प्रारंभ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/bymonthdayrepetition/bymonthdayrepetition/
---
## ByMonthDayRepetition constructor

[`ByMonthDayRepetition`](../) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public ByMonthDayRepetition()
```

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

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


