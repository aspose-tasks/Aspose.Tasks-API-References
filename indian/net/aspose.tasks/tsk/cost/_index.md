---
title: "Tsk.Cost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के लिए कुल नियोजित या अनुमानित लागत, जो उन संसाधनों द्वारा किए गए कार्य की पहले से हुई लागत और शेष कार्य के लिए नियोजित लागत दोनों पर आधारित है"
type: docs
weight: 230
url: /hi/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

कार्य के लिए कुल निर्धारित या अनुमानित लागत, जो कार्य को सौंपे गए संसाधनों द्वारा किए गए कार्य के लिए पहले से हुए खर्चों और शेष कार्य के लिए नियोजित खर्चों पर आधारित होती है।

```csharp
public static readonly Key<decimal, TaskKey> Cost;
```

## उदाहरण

कार्य लागत को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project();

// कार्य जोड़ें और लागत सेट करें
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// कार्य की लागत संबंधित प्रॉपर्टीज़ दिखाएँ
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


