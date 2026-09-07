---
title: "Tsk.OvertimeWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य को सौंपे गए सभी संसाधनों द्वारा किए जाने वाले ओवरटाइम की नियोजित मात्रा"
type: docs
weight: 870
url: /hi/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

किसी कार्य को असाइन किए गए सभी संसाधनों द्वारा किए जाने वाले निर्धारित ओवरटाइम की मात्रा।

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## उदाहरण

दिखाता है कि कैसे कार्य के ओवरटाइम को पढ़ा जाए।

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// कार्य के ओवरटाइम और प्रतिशत पूर्णता को पढ़ें
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // प्रतिशत पूर्णता सेट करें
    task.Set(Tsk.PercentComplete, 100);
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


