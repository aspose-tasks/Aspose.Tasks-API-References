---
title: "Calendar.GetIntersectionCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। ICalendar इंस्टेंस प्राप्त करता है जिसका उपयोग 2 कैलेंडरों के कार्य शेड्यूल के इंटरसेक्शन पर गणनाएँ करने के लिए किया जा सकता है"
type: docs
weight: 280
url: /hi/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

2 कैलेंडरों के कार्य शेड्यूल के इंटरसेक्शन पर गणनाएँ करने के लिए उपयोग किया जा सकने वाला [`ICalendar`](../../icalendar/) इंस्टेंस प्राप्त करता है।

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| calendar1 | कैलेंडर | पहला कैलेंडर। |
| calendar2 | कैलेंडर | दूसरा कैलेंडर। |

### रिटर्न वैल्यू

ICalendar इंटरफ़ेस का कार्यान्वयन।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | जब किसी भी तर्क का मान null हो। |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


