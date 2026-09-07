---
title: "Tsk.RemainingOvertimeWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। शेष नियोजित ओवरटाइम समय की मात्रा"
type: docs
weight: 980
url: /hi/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

शेष निर्धारित ओवरटाइम समय की मात्रा।

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## उदाहरण

दिखाता है कि Tsk.RemainingOvertimeWork प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


