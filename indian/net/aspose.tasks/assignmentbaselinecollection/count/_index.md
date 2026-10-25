---
title: "AssignmentBaselineCollection.Count"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AssignmentBaselineCollection प्रॉपर्टी। इस AssignmentBaselineCollection ऑब्जेक्ट में सम्मिलित ऑब्जेक्ट्स की संख्या प्राप्त करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

इस AssignmentBaselineCollection ऑब्जेक्ट में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है।

```csharp
public int Count { get; }
```

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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


