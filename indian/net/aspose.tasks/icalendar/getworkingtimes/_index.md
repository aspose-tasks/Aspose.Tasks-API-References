---
title: "ICalendar.GetWorkingTimes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ICalendar मेथड। निर्दिष्ट तिथि के लिए कार्य समयों की WorkingTimeCollection लौटाता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

निर्दिष्ट तिथि के लिए कार्य समयों की [`WorkingTimeCollection`](../../workingtimecollection/) लौटाता है।

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | DateTime | कार्य समय प्राप्त करने के लिए तिथि। |

### रिटर्न वैल्यू

[`WorkingTime`](../../workingtime/) के उदाहरणों का संग्रह।

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


