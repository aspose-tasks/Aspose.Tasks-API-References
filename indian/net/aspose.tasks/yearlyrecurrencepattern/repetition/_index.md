---
title: "YearlyRecurrencePattern.Repetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "YearlyRecurrencePattern प्रॉपर्टी। प्राप्त करता है या सेट करता है आवर्ती स्थिति पैटर्न"
type: docs
weight: 20
url: /hi/net/aspose.tasks/yearlyrecurrencepattern/repetition/
---
## YearlyRecurrencePattern.Repetition property

आवर्ती स्थिति पैटर्न को प्राप्त करता है या सेट करता है।

```csharp
public YearlyRepetitionBase Repetition { get; set; }
```

## उदाहरण

आवर्ती कार्य बनाते समय year year आवर्ती पैटर्न के साथ काम करने का तरीका दिखाता है।

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

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [YearlyRepetitionBase](../../yearlyrepetitionbase/)
* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


