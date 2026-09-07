---
title: "क्लास YearlyRecurrencePattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.YearlyRecurrencePattern क्लास. उन पैरामीटरों का सेट दर्शाता है जो प्रोजेक्ट में वार्षिक आवर्ती कार्य बनाने के लिए उपयोग किए जाते हैं।"
type: docs
weight: 3690
url: /hi/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

प्रोजेक्ट में वार्षिक आवर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट को दर्शाता है।

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | `YearlyRecurrencePattern` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | आवृत्ति रेंज को प्राप्त करता है या सेट करता है। |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | आवर्ती स्थिति पैटर्न को प्राप्त करता है या सेट करता है। |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


