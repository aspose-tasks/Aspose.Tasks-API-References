---
title: "Task.Set"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड। निर्दिष्ट प्रॉपर्टी को इस कंटेनर में निर्दिष्ट मान से मैप करता है।"
type: docs
weight: 1410
url: /hi/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | मैप किए गए मान का प्रकार। |
| key | निर्दिष्ट प्रॉपर्टी कुंजी। [`Tsk`](../../tsk/) प्रॉपर्टी कुंजी प्राप्त करने के लिए। |
| मान | मान। |

## उदाहरण

दिखाता है कि टास्क प्रॉपर्टीज़ को कैसे प्राप्त/सेट किया जाए।

```csharp
var project = new Project();

// कार्य जोड़ें और कार्य गुण सेट करें
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


