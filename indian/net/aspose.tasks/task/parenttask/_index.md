---
title: "Task.ParentTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task property. किसी कार्य का पैरेंट कार्य प्राप्त करता है"
type: docs
weight: 940
url: /hi/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

एक टास्क का पैरेंट टास्क प्राप्त करता है।

```csharp
public Task ParentTask { get; }
```

## उदाहरण

दिखाता है कि किसी कार्य का पैरेंट कार्य कैसे उपयोग किया जाए।

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


