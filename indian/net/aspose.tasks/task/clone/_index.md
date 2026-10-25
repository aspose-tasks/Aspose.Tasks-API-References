---
title: "Task.Clone"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड। सबटास्क के बिना टास्क की पूरी कॉपी बनाता है"
type: docs
weight: 1310
url: /hi/net/aspose.tasks/task/clone/
---
## Task.Clone method

सबटास्क के बिना टास्क की पूरी कॉपी बनाता है।

```csharp
public object Clone()
```

### रिटर्न वैल्यू

एक कार्य की प्रति बनाई गई।

## उदाहरण

दिखाता है कि कार्य को कैसे क्लोन किया जाए।

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


