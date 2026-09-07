---
title: "Tsk.PercentComplete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की वर्तमान स्थिति, जिसे कार्य की पूरी हुई अवधि के प्रतिशत के रूप में व्यक्त किया गया है"
type: docs
weight: 880
url: /hi/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

कार्य की वर्तमान स्थिति, जो कार्य की अवधि के पूर्ण किए गए प्रतिशत के रूप में व्यक्त की जाती है।

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## उदाहरण

दिखाता है कि कार्य की प्रगति को टास्क प्रतिशत पूर्णता को अपडेट करके कैसे बदलें।

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// कार्य तक पहुँचें और प्रतिशत पूर्णता प्रदर्शित करें
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


