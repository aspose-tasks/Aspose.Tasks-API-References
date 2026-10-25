---
title: "Resource.GetTimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource method. इस ऑब्जेक्ट के लिए TimephasedDataCollection क्लास का एक इंस्टेंस लौटाता है जिसमें निर्दिष्ट TimephasedDataType की दी गई प्रारंभ और समाप्ति तिथियों के भीतर TimephasedData मान होते हैं"
type: docs
weight: 850
url: /hi/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

इस ऑब्जेक्ट के लिए [`TimephasedDataCollection`](../../timephaseddatacollection/) क्लास का एक इंस्टेंस लौटाता है जिसमें [`TimephasedData`](../timephaseddata/) मान दिए गए प्रारंभ और समाप्ति तिथियों के भीतर निर्दिष्ट [`TimephasedDataType`](../../timephaseddatatype/) के होते हैं।

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

`[`TimephasedData`](../timephaseddata/)` की सूची।

## उदाहरण

कार्य/लागत संसाधनों के समय-फ़ेज़्ड डेटा को पढ़ने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// ID द्वारा Resource प्राप्त करें
var resource = project.Resources.GetByUid(1);

// ResourceWork का समय-फ़ेज़्ड डेटा प्रिंट करें
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// ResourceCost का समय-फ़ेज़्ड डेटा प्रिंट करें
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

इस ऑब्जेक्ट के लिए [`TimephasedDataCollection`](../../timephaseddatacollection/) लौटाता है जिसमें दिए गए प्रारंभ और समाप्ति तिथियों के भीतर [`TimephasedData`](../timephaseddata/) मान होते हैं।

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | समय-फ़ेज़्ड डेटा के लिए प्रारंभ तिथि। |
| समाप्ति | DateTime | समय-फ़ेज़्ड डेटा के लिए समाप्ति तिथि। |

### रिटर्न वैल्यू

`[`TimephasedData`](../../timephaseddata/)` की सूची।

## उदाहरण

कार्य/लागत संसाधनों के समय-फ़ेज़्ड डेटा को पढ़ने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// ID द्वारा Resource प्राप्त करें
var resource = project.Resources.GetByUid(1);

// ResourceWork का समय-फ़ेज़्ड डेटा प्रिंट करें
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// ResourceCost का समय-फ़ेज़्ड डेटा प्रिंट करें
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


