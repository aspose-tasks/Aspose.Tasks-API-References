---
title: "Tsk.Id"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्यों की सूची में किसी कार्य की स्थिति पहचानकर्ता"
type: docs
weight: 520
url: /hi/net/aspose.tasks/tsk/id/
---
## Tsk.Id field

कार्य सूची में कार्य की स्थिति पहचानकर्ता।

```csharp
public static readonly Key<int, TaskKey> Id;
```

## उदाहरण

दिखाता है कि कार्य गुणों को कैसे पढ़ें/लिखें।

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
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


