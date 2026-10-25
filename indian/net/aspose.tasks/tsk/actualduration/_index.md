---
title: "Tsk.ActualDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की वास्तविक कार्य समय की अवधि, जो निर्धारित अवधि और वर्तमान शेष कार्य या पूर्णता प्रतिशत पर आधारित है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

टास्क के वास्तविक कार्य समय की अवधि, निर्धारित अवधि और वर्तमान शेष कार्य या प्रतिशत पूर्णता के आधार पर।

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
```

## उदाहरण

दिखाता है कि कार्य की वास्तविक प्रॉपर्टीज़ को कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


