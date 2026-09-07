---
title: "SplitPart.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SplitPart मेथड। दो विभाजित भागों की तुलना करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/splitpart/equals/
---
## SplitPart.Equals method

दो स्प्लिट पार्ट्स की तुलना करता है।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | तुलना करने के लिए ऑब्जेक्ट। |

### रिटर्न वैल्यू

यदि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है तो सत्य; अन्यथा, असत्य।

## उदाहरण

विभाजित भागों की समानता की जाँच कैसे करें, दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(4));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("Resource"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// पहले संसाधन असाइनमेंट टाइम‑फ़ेज़ डेटा उत्पन्न करना आवश्यक है
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));
Console.WriteLine(assignment.Get(Asn.Finish));

// कार्य को विभाजित करें।
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// विभाजित भागों की समानता को शुरू, समाप्ति और सूचकांक के विरुद्ध जाँच किया जाता है।
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];
Console.WriteLine("Split Part 1 Start {0} Finish {1}", part1.Start, part1.Finish);
Console.WriteLine("Split Part 2 Start {0} Finish {1}", part2.Start, part2.Finish);
Console.WriteLine("Are split parts equal: " + part1.Equals(part2));
```

### संबंधित देखें

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


