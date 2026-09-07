---
title: "Task.OutlineOutdent"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task method. रूपरेखा में कार्य को प्रोन्नत करता है"
type: docs
weight: 1390
url: /hi/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

रूपरेखा में एक कार्य को प्रोमोट करता है।

```csharp
public void OutlineOutdent()
```

## उदाहरण

दिखाता है कि कार्य को आउटडेंट कैसे करें।

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// कार्य को आउटडेंट करें
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


