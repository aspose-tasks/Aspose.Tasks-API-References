---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। निर्दिष्ट TimephasedDataType की दी गई प्रारंभ और समाप्ति तिथियों के भीतर TimephasedData क्लास की इंस्टेंस को शामिल करने वाले TimephasedDataCollection क्लास की इंस्टेंस लौटाता है।"
type: docs
weight: 720
url: /hi/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

निर्दिष्ट [`TimephasedDataType`](../../timephaseddatatype/) की दी गई प्रारंभ और समाप्ति तिथियों के भीतर [`TimephasedData`](../timephaseddata/) क्लास की इंस्टेंस को शामिल करने वाले [`TimephasedDataCollection`](../../timephaseddatacollection/) क्लास की इंस्टेंस लौटाता है।

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | समय-फ़ेज़्ड डेटा के लिए प्रारंभ तिथि। |
| समाप्ति | DateTime | समय-फ़ेज़्ड डेटा के लिए समाप्ति तिथि। |
| timephasedType | TimephasedDataType | समय-फ़ेज़्ड डेटा का प्रकार ([`TimephasedDataType`](../../timephaseddatatype/)). |

### रिटर्न वैल्यू

एक सूची लौटाता है जिसमें [`TimephasedData`](../../timephaseddata/) क्लास की इंस्टेंस शामिल हैं।

## उदाहरण

एक डेट रेंज के भीतर रिसोर्स असाइनमेंट का समय-फ़ेज़्ड डेटा उत्पन्न करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// प्रोजेक्ट प्रॉपर्टीज़ सेट करें
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// रिसोर्स असाइनमेंट बनाएं
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Backloaded कॉन्टूर सेट करें, यह टास्क की अवधि को 6 से 10 दिनों तक बढ़ाता है।
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// समय-फ़ेज़्ड डेटा प्राप्त करें
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

निर्दिष्ट AssignmentWork की प्रारंभ और समाप्ति तिथियों के भीतर [`TimephasedData`](../timephaseddata/) क्लास की इंस्टेंस के साथ [`TimephasedDataCollection`](../../timephaseddatacollection/) ऑब्जेक्ट लौटाता है।

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | समय-फ़ेज़्ड डेटा के लिए प्रारंभ तिथि। |
| समाप्ति | DateTime | समय-फ़ेज़्ड डेटा के लिए समाप्ति तिथि। |

### रिटर्न वैल्यू

एक सूची लौटाता है जिसमें [`TimephasedData`](../../timephaseddata/) क्लास की इंस्टेंस शामिल हैं।

## उदाहरण

एक डेट रेंज के भीतर रिसोर्स असाइनमेंट का समय-फ़ेज़्ड डेटा उत्पन्न करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// प्रोजेक्ट प्रॉपर्टीज़ सेट करें
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// रिसोर्स असाइनमेंट बनाएं
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Backloaded कॉन्टूर सेट करें, यह टास्क की अवधि को 6 से 10 दिनों तक बढ़ाता है।
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// समय-फ़ेज़्ड डेटा प्राप्त करें
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


