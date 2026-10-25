---
title: "Tsk.RegularWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड. संसाधनों द्वारा किए जाने वाले गैर‑ओवरटाइम कार्य की कुल मात्रा निर्धारित।"
type: docs
weight: 940
url: /hi/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

संसाधनों द्वारा किए जाने वाले गैर‑ओवरटाइम कार्य की कुल निर्धारित मात्रा।

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## उदाहरण

Tsk.RegularWork प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


