---
title: "Tsk.ActualCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। संसाधनों द्वारा उनके कार्यों पर पहले किए गए कार्य के लिए उत्पन्न लागत, साथ ही कार्य से संबंधित किसी भी अन्य दर्ज लागत"
type: docs
weight: 20
url: /hi/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

संसाधनों द्वारा उनके टास्क पर पहले से किए गए कार्य के लिए हुई लागत, साथ ही टास्क से जुड़े किसी भी अन्य दर्ज लागत।

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


