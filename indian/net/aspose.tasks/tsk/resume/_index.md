---
title: "Tsk.Resume"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह तिथि जब कार्य का शेष भाग किसी प्रगति में प्रवेश करने के बाद पुनः शुरू होने के लिए निर्धारित है"
type: docs
weight: 1000
url: /hi/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

कार्य के शेष भाग के किसी भी प्रगति में प्रवेश करने के बाद पुनः शुरू होने की निर्धारित तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
```

## उदाहरण

दिखाता है कि कार्य की Stop/Resume तिथियों को कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी कार्यों के लिए Stop और Resume तिथियों की जाँच करें
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


