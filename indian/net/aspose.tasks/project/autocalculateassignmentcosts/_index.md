---
title: "Project.AutoCalculateAssignmentCosts"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। यह प्राप्त करता है या सेट करता है कि असाइनमेंट लागत और शेष लागत को असाइनमेंट कार्य और संसाधन दरों का उपयोग करके स्वचालित रूप से गणना किया जाना चाहिए या नहीं।"
type: docs
weight: 70
url: /hi/net/aspose.tasks/project/autocalculateassignmentcosts/
---
## Project.AutoCalculateAssignmentCosts property

असाइनमेंट की कार्य और रिसोर्स रेट्स का उपयोग करके असाइनमेंट लागत और शेष लागत को स्वतः गणना किया जाना चाहिए या नहीं, यह प्राप्त करता है या सेट करता है।

```csharp
public bool AutoCalculateAssignmentCosts { get; set; }
```

## उदाहरण

असाइनमेंट लागत की स्वचालित गणना को बंद करने और लागत को स्पष्ट रूप से सेट करने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("New task");
task.Duration = project.GetDuration(TimeSpan.FromHours(15), TimeUnitType.Day);
var resource = project.Resources.Add("Resource");
resource.StandardRate = 10m;

var assignment = project.ResourceAssignments.Add(task, resource);

assignment.Work = project.GetDuration(TimeSpan.FromHours(12), TimeUnitType.Day);
assignment.ActualWork = project.GetDuration(TimeSpan.FromHours(3), TimeUnitType.Day);

Console.WriteLine("Now assignment's cost are auto calculated:");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);

project.AutoCalculateAssignmentCosts = false;
assignment.ActualCost = 123;
assignment.RemainingCost = 456;
assignment.Cost = 555;

Console.WriteLine("Now auto calculation of assignment's cost is turned off.");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


