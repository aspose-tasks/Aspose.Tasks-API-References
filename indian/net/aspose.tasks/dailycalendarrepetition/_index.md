---
title: "क्लास DailyCalendarRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.DailyCalendarRepetition क्लास। कैलेंडर दिनों के आधार पर दैनिक पुनरावृत्ति पैटर्न में पुनरावृत्तियों के लिए एक क्लास का प्रतिनिधित्व करता है"
type: docs
weight: 390
url: /hi/net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

कैलेंडर दिनों पर आधारित दैनिक पुनरावृत्ति पैटर्न में दोहराव के लिए एक क्लास का प्रतिनिधित्व करता है।

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | `DailyCalendarRepetition` क्लास की नई instance को इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | घटनाओं के बीच दिनों में अंतराल को दर्शाने वाले दिनों की संख्या को प्राप्त करता है या सेट करता है। |

## उदाहरण

दैनिक कार्य पुनरावृत्ति पैटर्न की पुनरावृत्तियों और '24 घंटे' के साथ आवर्ती कार्य बनाने के दौरान कैसे काम करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");
var calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(calendar);
var parameters = new RecurringTaskParameters
{
    TaskName = "t1",
    Duration = project.GetDuration(1, TimeUnitType.Day),
    RecurrencePattern = new DailyRecurrencePattern
    {
        Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
        RecurrenceRange = new EndByRecurrenceRange
        {
            Start = new DateTime(2018, 7, 2, 0, 0, 0),
            Finish = new DateTime(2018, 7, 8, 16, 0, 0)
        }
    }
};
parameters.SetCalendar(project, "24 Hours");
project.RootTask.Children.Add(parameters);

// परियोजना के साथ आगे काम करें...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


