---
title: "Tsk.OvertimeCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. किसी संसाधन के सभी असाइन किए गए कार्यों या संसाधन असाइनमेंट पर कार्य के लिए कुल ओवरटाइम लागत"
type: docs
weight: 860
url: /hi/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

किसी कार्य, सभी असाइन किए गए कार्यों पर किसी संसाधन, या किसी संसाधन असाइनमेंट के लिए कुल ओवरटाइम लागत।

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


