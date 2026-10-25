---
title: "क्लास TimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TimephasedData क्लास। समय-फ़ेज़्ड डेटा दर्शाता है"
type: docs
weight: 2590
url: /hi/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

समय-फ़ेज़्ड डेटा का प्रतिनिधित्व करता है।

```csharp
public class TimephasedData
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TimephasedData](timephaseddata/)() | `TimephasedData` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | समय-फ़ेज़्ड डेटा अवधि की समाप्ति तिथि प्राप्त करता या सेट करता है। |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | समय-फ़ेज़्ड डेटा अवधि की प्रारंभ तिथि प्राप्त करता या सेट करता है। |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | समय-फ़ेज़्ड डेटा का प्रकार प्राप्त करता या सेट करता है। |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | समय-फ़ेज़्ड डेटा का अद्वितीय पहचानकर्ता प्राप्त करता या सेट करता है |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | समय-फ़ेज़्ड डेटा अवधि की समय इकाई प्राप्त करता या सेट करता है। |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | समय-फ़ेज़्ड डेटा अवधि के लिए प्रति समय इकाई मान प्राप्त करता या सेट करता है। |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | डबल इंस्टेंस प्राप्त करता है जो इस ऑब्जेक्ट का स्ट्रिंग मान दर्शाता है। |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | टाइमस्पैन इंस्टेंस प्राप्त करता है जो इस ऑब्जेक्ट का स्ट्रिंग मान दर्शाता है। |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | यूनिट-आधारित समय-फ़ेज़्ड डेटा के लिए इस ऑब्जेक्ट का स्ट्रिंग मान दर्शाने वाला डबल इंस्टेंस प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | `TimephasedData` क्लास का नया उदाहरण बनाता और प्रारंभ करता है लागत-आधारित समय-फ़ेज़्ड डेटा के लिए। |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | `TimephasedData` क्लास का नया उदाहरण बनाता और प्रारंभ करता है लागत-आधारित समय-फ़ेज़्ड डेटा के लिए। |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | `TimephasedData` क्लास का नया उदाहरण बनाता और प्रारंभ करता है सामग्री संसाधन के असाइनमेंट के यूनिट-आधारित समय-फ़ेज़्ड डेटा के लिए। |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | काम-आधारित समय-फ़ेज़्ड डेटा के लिए `TimephasedData` क्लास का नया उदाहरण बनाता और प्रारंभ करता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


