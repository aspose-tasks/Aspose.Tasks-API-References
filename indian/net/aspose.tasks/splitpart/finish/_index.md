---
title: "SplitPart.Finish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SplitPart प्रॉपर्टी। SplitPart की समाप्ति तिथि प्राप्त करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/splitpart/finish/
---
## SplitPart.Finish property

एक SplitPart की समाप्ति तिथि प्राप्त करता है।

```csharp
public DateTime Finish { get; }
```

## उदाहरण

विभाजित कार्य के स्प्लिट पार्ट्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// पहले संसाधन असाइनमेंट टाइम‑फ़ेज़ डेटा उत्पन्न करना आवश्यक है
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// कार्य को विभाजित करें।
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// स्प्लिट पार्ट्स पर इटरेट करें
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### संबंधित देखें

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


