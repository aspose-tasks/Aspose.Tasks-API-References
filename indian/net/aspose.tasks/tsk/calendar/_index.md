---
title: "Tsk.Calendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य कैलेंडर"
type: docs
weight: 160
url: /hi/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

टास्क कैलेंडर।

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## उदाहरण

कार्य कैलेंडर को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// कैलेंडर बनाएं और कार्य को असाइन करें
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी पुनरावर्ती चाइल्ड को पार्स करें
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


