---
title: "क्लास AssignmentBaselineCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.AssignmentBaselineCollection class. AssignmentBaseline ऑब्जेक्ट्स का एक संग्रह दर्शाता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

[`AssignmentBaseline`](../assignmentbaseline/) ऑब्जेक्ट्स का एक संग्रह दर्शाता है।

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | इस AssignmentBaselineCollection ऑब्जेक्ट में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | इस संग्रह के लिए पैरेंट [`ResourceAssignment`](../resourceassignment/) प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकती है। |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | इस संग्रह से बेसलाइन को हटाता है। |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | AssignmentBaselineCollection ऑब्जेक्ट को [`AssignmentBaseline`](../assignmentbaseline/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


