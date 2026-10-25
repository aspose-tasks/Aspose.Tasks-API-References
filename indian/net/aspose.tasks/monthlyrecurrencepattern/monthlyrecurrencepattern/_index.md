---
title: "MonthlyRecurrencePattern.MonthlyRecurrencePattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MonthlyRecurrencePattern कंस्ट्रक्टर। MonthlyRecurrencePattern क्लास का एक नया इंस्टेंस प्रारंभ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/monthlyrecurrencepattern/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern constructor

[`MonthlyRecurrencePattern`](../) क्लास का एक नया इंस्टेंस प्रारंभ करता है।

```csharp
public MonthlyRecurrencePattern()
```

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

* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


