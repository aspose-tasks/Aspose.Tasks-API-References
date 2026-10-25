---
title: "Tsk.ActualWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। उन संसाधनों द्वारा किए गए कार्य की मात्रा जो कार्यों को असाइन किए गए हैं"
type: docs
weight: 90
url: /hi/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

टास्क को सौंपे गए संसाधनों द्वारा पहले से किए गए कार्य की मात्रा।

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## उदाहरण

Tsk.ActualWork प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


