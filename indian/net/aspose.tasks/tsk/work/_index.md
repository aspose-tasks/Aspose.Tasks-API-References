---
title: "Tsk.Work"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड. सभी नियोजित संसाधनों के लिए कार्य पर निर्धारित कुल समय।"
type: docs
weight: 1150
url: /hi/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

सभी असाइन किए गए संसाधनों के लिए कार्य पर निर्धारित कुल समय।

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## उदाहरण

Tsk.Work प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


