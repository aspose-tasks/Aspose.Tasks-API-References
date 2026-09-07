---
title: "ResourceAssignment.Delete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment विधि. प्रोजेक्ट असाइनमेंट्स संग्रह से संसाधन असाइनमेंट को हटाता है"
type: docs
weight: 680
url: /hi/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

प्रोजेक्ट असाइनमेंट संग्रह से संसाधन असाइनमेंट को हटाता है।

```csharp
public void Delete()
```

## उदाहरण

दिखाता है कि कैसे एक संसाधन असाइनमेंट को हटाया जाए.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### संबंधित देखें

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


