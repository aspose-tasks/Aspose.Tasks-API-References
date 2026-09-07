---
title: "TimephasedData.CreateUnitTimephased"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TimephasedData मेथड। एक सामग्री संसाधन के असाइनमेंट के यूनिट-आधारित समय-फ़ेज़्ड डेटा के लिए TimephasedData क्लास का एक नया इंस्टेंस बनाता और प्रारंभ करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/timephaseddata/createunittimephased/
---
## TimephasedData.CreateUnitTimephased method

एक सामग्री संसाधन के असाइनमेंट के यूनिट-आधारित समय-फ़ेज़्ड डेटा के लिए [`TimephasedData`](../) क्लास का एक नया इंस्टेंस बनाता और प्रारंभ करता है।

```csharp
public static TimephasedData CreateUnitTimephased(int uid, DateTime start, DateTime finish, 
    double units, TimephasedDataType type)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | Int32 | टास्क का UID। |
| प्रारंभ | DateTime | प्रारंभ तिथि-समय। |
| समाप्ति | DateTime | समाप्ति तिथि-समय। |
| इकाइयाँ | Double | इकाइयों की संख्या। |
| प्रकार | TimephasedDataType | समय-फ़ेज़्ड डेटा प्रकार। |

### रिटर्न वैल्यू

लागत-आधारित समय-फ़ेज़्ड डेटा के लिए [`TimephasedData`](../) क्लास का एक इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | यदि इकाइयों की नकारात्मक मात्रा निर्दिष्ट की गई थी। |

## उदाहरण

कस्टम टाइमफ़ेज़्ड डेटा के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp") { CalculationMode = CalculationMode.None };

var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2018, 1, 1, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var workAssignment = project.ResourceAssignments.Add(task, workResource);
workAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);
var costAssignment = project.ResourceAssignments.Add(task, costResource);
costAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);

// आइए कस्टम टाइमफ़ेज़्ड टीडीएस जोड़ें
workAssignment.TimephasedData.Clear();

// कार्य दिवस जोड़ें
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// सप्ताहांत जोड़ें
var td2 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    TimeSpan.Zero,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

workAssignment.TimephasedData.Add(td1);
workAssignment.TimephasedData.Add(td2);

costAssignment.TimephasedData.Clear();

// कार्य दिवस जोड़ें
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// सप्ताहांत जोड़ें
var td22 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    0,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

costAssignment.TimephasedData.Add(td11);
costAssignment.TimephasedData.Add(td22);

Console.WriteLine("Print assignment timephased data:");
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
    foreach (var tds in assignment.TimephasedData)
    {
        Console.WriteLine("  Uid: " + tds.Uid);
        Console.WriteLine("  Start: " + tds.Start);
        Console.WriteLine("  Finish: " + tds.Finish);
        Console.WriteLine("  Type: " + tds.TimephasedDataType);
        Console.WriteLine("  Unit: " + tds.Unit);
        Console.WriteLine("  Value: " + tds.Value);
        Console.WriteLine("  ValueToCost: " + tds.ValueToCost);
        Console.WriteLine("  ValueToDuration: " + tds.ValueToDuration);
        Console.WriteLine("  ValueToUnits: " + tds.ValueToUnits);
        Console.WriteLine();
    }
}

project.Recalculate();
```

### संबंधित देखें

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)


