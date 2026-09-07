---
title: "AssignmentBaselineCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AssignmentBaselineCollection मेथड। AssignmentBaselineCollection ऑब्जेक्ट को AssignmentBaseline ऑब्जेक्ट्स की सूची में परिवर्तित करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

AssignmentBaselineCollection ऑब्जेक्ट को [`AssignmentBaseline`](../../assignmentbaseline/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

```csharp
public List<AssignmentBaseline> ToList()
```

### रिटर्न वैल्यू

[`AssignmentBaseline`](../../assignmentbaseline/) ऑब्जेक्ट्स की सूची।

## उदाहरण

असाइनमेंट बेसलाइन पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// असाइनमेंट बेसलाइन जानकारी पढ़ें
foreach (var assignment in project.ResourceAssignments)
{
    var baselines = assignment.Baselines;
    Console.WriteLine("Count of assignment baselines: " + baselines.Count);
    Console.WriteLine("Parent Assignment: " + baselines.ParentAssignment);
    foreach (var baseline in baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
    }

    Console.WriteLine();
}

Console.WriteLine("Delete all assignment baselines: ");

// असाइनमेंट बेसलाइन हटाएँ
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### संबंधित देखें

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


