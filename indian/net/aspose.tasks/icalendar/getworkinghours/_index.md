---
title: "ICalendar.GetWorkingHours"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ICalendar मेथड। निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की WorkUnit प्रारंभ, समाप्ति और अवधि लौटाता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की WorkUnit - प्रारंभ, समाप्ति और अवधि लौटाता है।

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | अंतराल की प्रारंभ तिथि। |
| समाप्ति | DateTime | अंतराल की समाप्ति तिथि। |

### रिटर्न वैल्यू

[`WorkUnit`](../../workunit/) क्लास का उदाहरण जिसमें कार्य घंटे की प्रारंभ, समाप्ति और अवधि शामिल है।

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

निर्दिष्ट तिथि पर कार्य घंटे की मात्रा लौटाता है।

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | DateTime | कार्य घंटे प्राप्त करने के लिए तिथि। |

### रिटर्न वैल्यू

निर्दिष्ट तिथि पर कार्य घंटे।

### संबंधित देखें

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


