---
title: "ResourceAssignment.Baselines"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment property. AssignmentBaselineCollection ऑब्जेक्ट प्राप्त करता है। वह संग्रह जिसमें असाइनमेंट से जुड़े बेसलाइन मान होते हैं"
type: docs
weight: 120
url: /hi/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

AssignmentBaselineCollection ऑब्जेक्ट प्राप्त करता है। असाइनमेंट से जुड़े बेसलाइन मानों का संग्रह।

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## उदाहरण

दिखाता है कि असाइनमेंट की बेसलाइन तक कैसे पहुँच प्राप्त की जाए।

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### संबंधित देखें

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


