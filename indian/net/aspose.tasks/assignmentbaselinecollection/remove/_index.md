---
title: "AssignmentBaselineCollection.Remove"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AssignmentBaselineCollection मेथड। इस संग्रह से बेसलाइन हटाता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

इस संग्रह से बेसलाइन को हटाता है।

```csharp
public bool Remove(AssignmentBaseline item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आइटम | AssignmentBaseline | हटाने के लिए आइटम। |

### रिटर्न वैल्यू

यदि [`AssignmentBaseline`](../../assignmentbaseline/) का उदाहरण सफलतापूर्वक हटाया गया हो तो true; अन्यथा false

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


