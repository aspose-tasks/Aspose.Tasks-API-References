---
title: "Task.Predecessors"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। एक TaskCollection ऑब्जेक्ट प्राप्त करता है जिसमें इस Task ऑब्जेक्ट के सभी पूर्वज शामिल होते हैं"
type: docs
weight: 980
url: /hi/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

एक [`TaskCollection`](../../taskcollection/) ऑब्जेक्ट प्राप्त करता है जिसमें इस Task ऑब्जेक्ट के सभी पूर्वज शामिल होते हैं।

```csharp
public TaskCollection Predecessors { get; }
```

### रिटर्न वैल्यू

केवल-पढ़ने योग्य इंस्टेंस [`TaskCollection`](../../taskcollection/) क्लास का।

## उदाहरण

दिखाता है कि कार्य के पूर्वजों को कैसे पढ़ा जाए।

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### संबंधित देखें

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


