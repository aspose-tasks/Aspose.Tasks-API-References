---
title: "Tsk.ActualStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह तिथि और समय जब कार्य वास्तव में शुरू हुआ"
type: docs
weight: 80
url: /hi/net/aspose.tasks/tsk/actualstart/
---
## Tsk.ActualStart field

टास्क के वास्तविक रूप से शुरू होने की तिथि और समय।

```csharp
public static readonly Key<DateTime, TaskKey> ActualStart;
```

## उदाहरण

दिखाता है कि प्रोजेक्ट की तिथियां मूल्यांकन मोड में रीसेट की गई हैं।

```csharp
var project = new Project();

// नए कार्य बनाएं
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


