---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह अवधि जिसके दौरान वास्तविक ओवरटाइम कार्य संरक्षित रहता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

वास्तविक ओवरटाइम कार्य की सुरक्षा की अवधि।

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## उदाहरण

दिखाता है कि Tsk.ActualOvertimeWorkProtected प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


