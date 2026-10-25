---
title: "Tsk.FixedCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। किसी भी गैर‑संसाधन कार्य खर्च को दिखाता है"
type: docs
weight: 430
url: /hi/net/aspose.tasks/tsk/fixedcost/
---
## Tsk.FixedCost field

कोई भी गैर-संसाधन कार्य व्यय दिखाता है।

```csharp
public static readonly Key<double, TaskKey> FixedCost;
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


