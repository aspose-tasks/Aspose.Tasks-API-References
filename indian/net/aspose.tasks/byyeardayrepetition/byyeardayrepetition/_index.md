---
title: "ByYearDayRepetition.ByYearDayRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ByYearDayRepetition कंस्ट्रक्टर। ByYearDayRepetition क्लास का नया उदाहरण इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/byyeardayrepetition/byyeardayrepetition/
---
## ByYearDayRepetition constructor

नया उदाहरण इनिशियलाइज़ करता है [`ByYearDayRepetition`](../) क्लास का।

```csharp
public ByYearDayRepetition()
```

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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


