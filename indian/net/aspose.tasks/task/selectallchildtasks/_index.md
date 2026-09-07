---
title: "Task.SelectAllChildTasks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड। इस टास्क के सभी चाइल्ड टास्क को पुनरावर्ती रूप से एकत्र करता है"
type: docs
weight: 1400
url: /hi/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

इस कार्य के सभी चाइल्ड कार्यों को पुनरावर्ती रूप से एकत्र करता है।

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### रिटर्न वैल्यू

इस टास्क के चाइल्ड टास्क की सूची।

## उदाहरण

चाइल्ड टास्क पर इटरेट करने का तरीका दिखाता है।

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


