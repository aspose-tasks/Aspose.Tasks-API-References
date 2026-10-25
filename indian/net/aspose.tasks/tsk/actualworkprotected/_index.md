---
title: "Tsk.ActualWorkProtected"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड. वास्तविक कार्य की सुरक्षा अवधि। पढ़ना केवल XML फ़ॉर्मेट के लिए समर्थित है।"
type: docs
weight: 100
url: /hi/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

वास्तविक कार्य की सुरक्षा की अवधि। केवल XML फ़ॉर्मेट के लिए पढ़ना समर्थित है।

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## उदाहरण

Tsk.ActualWorkProtected प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


