---
title: "Tsk.RemainingWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। किसी कार्य या कार्य समूह को पूरा करने के लिए अभी भी आवश्यक समय"
type: docs
weight: 990
url: /hi/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

किसी कार्य या कार्य समूह को पूरा करने के लिए अभी भी आवश्यक समय।

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## उदाहरण

Tsk.RemainingWork प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


