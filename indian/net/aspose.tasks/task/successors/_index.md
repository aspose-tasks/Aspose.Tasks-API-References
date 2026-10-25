---
title: "Task.Successors"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task property. प्राप्त करता है एक TaskCollection ऑब्जेक्ट जो इस Task ऑब्जेक्ट के सभी उत्तराधिकारियों को शामिल करता है"
type: docs
weight: 1200
url: /hi/net/aspose.tasks/task/successors/
---
## Task.Successors property

एक [`TaskCollection`](../../taskcollection/) ऑब्जेक्ट प्राप्त करता है जो इस Task ऑब्जेक्ट के सभी उत्तराधिकारियों को शामिल करता है।

```csharp
public TaskCollection Successors { get; }
```

### रिटर्न वैल्यू

केवल-पढ़ने योग्य इंस्टेंस [`TaskCollection`](../../taskcollection/) क्लास का।

## उदाहरण

दिखाता है कि टास्क के उत्तराधिकारियों को कैसे पढ़ा जाए।

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### संबंधित देखें

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


