---
title: "ResourceAssignment.ParentProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment प्रॉपर्टी। इस असाइनमेंट के लिए पैरेंट प्रोजेक्ट प्राप्त करता है।"
type: docs
weight: 420
url: /hi/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

इस असाइनमेंट के लिए पैरेंट प्रोजेक्ट प्राप्त करता है।

```csharp
public Project ParentProject { get; }
```

## उदाहरण

रिसोर्स असाइनमेंट के पैरेंट प्रोजेक्ट का उपयोग कैसे करें, यह दिखाता है।

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// डिफ़ॉल्ट प्रोजेक्ट टाइम यूनिट टाइप का उपयोग करके असाइनमेंट की अवधि सेट करें।
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### संबंधित देखें

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


