---
title: "Task.ParentProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। कार्य का पैरेंट प्रोजेक्ट प्राप्त करता है।"
type: docs
weight: 930
url: /hi/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

एक टास्क का पैरेंट प्रोजेक्ट प्राप्त करता है।

```csharp
public Project ParentProject { get; }
```

## टिप्पणियाँ

इन प्रॉपर्टीज़ को अपडेट करने के लिए Project.UpdateReferences को कॉल करें।

## उदाहरण

कार्य के पैरेंट प्रोजेक्ट का उपयोग करने का तरीका दिखाता है।

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// डिफ़ॉल्ट प्रोजेक्ट टाइम यूनिट टाइप का उपयोग करके कार्य की अवधि सेट करें।
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### संबंधित देखें

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


