---
title: "Tsk.Priority"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य को दिया गया महत्व स्तर जो यह दर्शाता है कि संसाधन लेवलिंग के दौरान कार्य या असाइनमेंट को कितनी आसानी से विलंबित या विभाजित किया जा सकता है"
type: docs
weight: 930
url: /hi/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

कार्य को दिया गया महत्व स्तर, जो यह दर्शाता है कि संसाधन लेवलिंग के दौरान कार्य या असाइनमेंट को कितनी आसानी से विलंब या विभाजित किया जा सकता है।

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## उदाहरण

दिखाता है कि कार्य प्राथमिकता को कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी कार्यों के लिए प्राथमिकताएँ प्रदर्शित करें
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


