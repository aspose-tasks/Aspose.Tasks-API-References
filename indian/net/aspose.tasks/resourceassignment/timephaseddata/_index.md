---
title: "ResourceAssignment.TimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment प्रॉपर्टी। प्राप्त करता है या सेट करता है TimephasedDataCollection क्लास का इंस्टेंस जिसमें TimephasedData क्लास के तत्व होते हैं"
type: docs
weight: 600
url: /hi/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

प्राप्त करता है या सेट करता है [`TimephasedDataCollection`](../../timephaseddatacollection/) क्लास का इंस्टेंस जिसमें `TimephasedData` क्लास के तत्व होते हैं।

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## उदाहरण

दिखाता है कि कैसे एक रिसोर्स असाइनमेंट का टाइमफ़ेज़्ड डेटा पढ़ा जाए।

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
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
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// समय-फ़ेज़्ड डेटा प्राप्त करें
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


