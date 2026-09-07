---
title: "ByYearDayRepetition.DayPosition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ByYearDayRepetition प्रॉपर्टी। प्राप्त करता है या सेट करता है महीने में दिन की वह स्थिति जिसमें टास्क को दोहराना चाहिए।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/byyeardayrepetition/dayposition/
---
## ByYearDayRepetition.DayPosition property

कार्य को पुनरावर्ती करने के लिए महीने में दिन की स्थिति प्राप्त करता है या सेट करता है।

```csharp
public int DayPosition { get; set; }
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


