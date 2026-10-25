---
title: "Tsk.PercentWorkComplete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की वर्तमान स्थिति, जो पूर्ण किए गए कार्य के प्रतिशत के रूप में व्यक्त की गई है"
type: docs
weight: 890
url: /hi/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

कार्य की वर्तमान स्थिति, जो पूर्ण किए गए कार्य के प्रतिशत के रूप में व्यक्त की जाती है।

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## उदाहरण

Tsk.PercentWorkComplete प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


