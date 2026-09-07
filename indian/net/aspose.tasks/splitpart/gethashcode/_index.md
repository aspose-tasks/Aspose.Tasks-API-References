---
title: "SplitPart.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SplitPart मेथड। SplitPart क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

`[`SplitPart`](../)` क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

विभाजित भाग का हैश कोड कैसे प्राप्त करें, दिखाता है।

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

// विभाजित भागों की समानता को शुरू, समाप्ति और सूचकांक के विरुद्ध जाँच किया जाता है।
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// विभाजित भाग का हैश कोड, जो शुरू, समाप्ति और सूचकांक पर आधारित है।
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### संबंधित देखें

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


