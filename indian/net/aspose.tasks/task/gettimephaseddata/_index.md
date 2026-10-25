---
title: "Task.GetTimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड। निर्दिष्ट timephased डेटा प्रकार की दी गई शुरू और समाप्ति तिथियों के भीतर TimephasedData मानों के साथ TimephasedDataCollection ऑब्जेक्ट लौटाता है।"
type: docs
weight: 1360
url: /hi/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

दिए गए शुरू और समाप्ति तिथियों के भीतर निर्दिष्ट time‑phased डेटा प्रकार के साथ [`TimephasedDataCollection`](../../timephaseddatacollection/) ऑब्जेक्ट लौटाता है, जिसमें [`TimephasedData`](../timephaseddata/) मान होते हैं।

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

एक [`TimephasedDataCollection`](../../timephaseddatacollection/) ऑब्जेक्ट जिसमें निर्दिष्ट timephased डेटा प्रकार की दी गई शुरू और समाप्ति तिथियों के भीतर [`TimephasedData`](../timephaseddata/) मान होते हैं।

## उदाहरण

दिखाता है कि कार्य का timephased डेटा (विशिष्ट प्रकार के साथ) कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

दिए गए शुरू और समाप्ति तिथियों के भीतर [`TimephasedData`](../timephaseddata/) मानों के साथ [`TimephasedDataCollection`](../../timephaseddatacollection/) ऑब्जेक्ट लौटाता है।

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | समय-फ़ेज़्ड डेटा के लिए प्रारंभ तिथि। |
| समाप्ति | DateTime | समय-फ़ेज़्ड डेटा के लिए समाप्ति तिथि। |

### रिटर्न वैल्यू

भरण के लिए [`TimephasedData`](../../timephaseddata/) की सूची।

## उदाहरण

कार्य की टाइमफ़ेज़्ड डेटा (TaskWork प्रकार के साथ) प्राप्त करने का तरीका दिखाता है।

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


