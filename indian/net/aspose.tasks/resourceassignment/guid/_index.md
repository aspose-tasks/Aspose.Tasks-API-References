---
title: "ResourceAssignment.Guid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment प्रॉपर्टी। इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता प्राप्त करता है या सेट करता है"
type: docs
weight: 290
url: /hi/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

इस असाइनमेंट के लिए अद्वितीय पहचानकर्ता प्राप्त करता है या सेट करता है।

```csharp
public Guid? Guid { get; set; }
```

## उदाहरण

दिखाता है कि कैसे एक रिसोर्स असाइनमेंट GUID पढ़ा जाए।

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### संबंधित देखें

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


