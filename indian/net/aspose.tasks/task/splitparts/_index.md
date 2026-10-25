---
title: "Task.SplitParts"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। एक SplitPart कलेक्शन प्राप्त करता है जो टास्क के भागों को दर्शाता है"
type: docs
weight: 1110
url: /hi/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

एक SplitPart संग्रह प्राप्त करता है जो टास्क के भागों को दर्शाता है।

```csharp
public SplitPartCollection SplitParts { get; }
```

## उदाहरण

दिखाता है कि टास्क के विभाजित भागों को कैसे प्रदर्शित किया जाए।

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// टास्क तक पहुँचें 
var task = project.RootTask.Children.GetById(4);

// टास्क के विभाजित भागों को प्रदर्शित करें
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### संबंधित देखें

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


