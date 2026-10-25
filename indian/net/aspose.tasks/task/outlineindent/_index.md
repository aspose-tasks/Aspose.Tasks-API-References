---
title: "Task.OutlineIndent"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task method. रूपरेखा में एक कार्य को इंडेंट करता है"
type: docs
weight: 1380
url: /hi/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

रूपरेखा में एक कार्य को इंडेंट करता है।

```csharp
public void OutlineIndent()
```

## उदाहरण

दिखाता है कि कार्य को कैसे इंडेंट किया जाए।

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// कार्य को इंडेंट करें
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


