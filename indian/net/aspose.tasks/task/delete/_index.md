---
title: "Task.Delete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड। टास्क को पैरेंट प्रोजेक्ट टास्क कलेक्शन और सभी असाइनमेंट्स से हटाता है।"
type: docs
weight: 1320
url: /hi/net/aspose.tasks/task/delete/
---
## Task.Delete method

पेरेंट प्रोजेक्ट टास्क संग्रह से टास्क और उसकी सभी असाइनमेंट हटाता है।

```csharp
public void Delete()
```

## उदाहरण

दिखाता है कि टास्क को कैसे हटाया जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// टास्क हटाएँ
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


