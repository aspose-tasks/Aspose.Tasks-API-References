---
title: "Resource.TimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी। इस ऑब्जेक्ट के लिए TimephasedDataCollection क्लास का एक इंस्टेंस प्राप्त करता है या सेट करता है"
type: docs
weight: 740
url: /hi/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

इस वस्तु के लिए [`TimephasedDataCollection`](../../timephaseddatacollection/) क्लास का एक उदाहरण प्राप्त करता है या सेट करता है।

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## टिप्पणियाँ

पढ़ना केवल XML फ़ॉर्मेट के लिए समर्थित है।

## उदाहरण

संसाधन के समय-फ़ेज़्ड डेटा को पढ़ने का तरीका दिखाता है।

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// संसाधन के समय-फ़ेज़्ड डेटा पर इटरेट करें।
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


