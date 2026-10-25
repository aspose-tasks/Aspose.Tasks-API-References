---
title: "इंटरफ़ेस ICalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ICalendar इंटरफ़ेस। एक कैलेंडर एब्स्ट्रैक्शन का प्रतिनिधित्व करता है जिसका उपयोग तिथियों और अवधियों की विभिन्न गणनाओं के लिए किया जा सकता है।"
type: docs
weight: 840
url: /hi/net/aspose.tasks/icalendar/
---
## ICalendar interface

तारीखों और अवधियों की विभिन्न गणनाओं के लिए उपयोग की जा सकने वाली कैलेंडर एब्स्ट्रैक्शन का प्रतिनिधित्व करता है।

```csharp
public interface ICalendar
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने पर तिथि की गणना करता है। |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने पर तिथि की गणना करता है। |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है। |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | निर्दिष्ट तिथि से पिछले कार्य दिवस के अंत की गणना करता है। |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है। |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है। |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | कार्य की प्रारंभ तिथि, विभाजित भागों और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है। |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | निर्दिष्ट तिथि पर कार्य घंटे की मात्रा लौटाता है। |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की WorkUnit - प्रारंभ, समाप्ति और अवधि लौटाता है। |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | निर्दिष्ट तिथियों के बीच कार्य घंटे की मात्रा लौटाता है। |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | निर्दिष्ट तिथि के लिए कार्य समय की [`WorkingTimeCollection`](../workingtimecollection/) लौटाता है। |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | निर्दिष्ट तिथि और समय से शुरू होकर अगले कार्य समय की शुरुआत की गणना करता है। |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | कैलेंडर के अनुसार निर्धारित करता है कि निर्दिष्ट दिन कार्य दिवस है या नहीं। |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | वापस देता है कि क्या कैलेंडर में कार्य घंटे परिभाषित नहीं हैं। |

## उदाहरण

असाइनमेंट के कैलेंडर पर गणना करने के लिए Calendar.GetIntersectionCalendar() मेथड का उपयोग कैसे किया जाए, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


