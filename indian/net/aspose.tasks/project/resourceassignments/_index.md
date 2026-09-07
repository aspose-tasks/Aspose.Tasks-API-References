---
title: "Project.ResourceAssignments"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। ResourceAssignmentCollection ऑब्जेक्ट प्राप्त करता है"
type: docs
weight: 750
url: /hi/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

ResourceAssignmentCollection ऑब्जेक्ट प्राप्त करता है।

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## उदाहरण

रिसोर्स असाइनमेंट्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();

// नया टास्क और रिसोर्स जोड़ें
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// रिसोर्स को इच्छित कार्य असाइन करें
project.ResourceAssignments.Add(task, resource);
```

### संबंधित देखें

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


