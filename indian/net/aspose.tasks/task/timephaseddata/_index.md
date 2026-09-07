---
title: "Task.TimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। इस कार्य की TimephasedDataCollection ऑब्जेक्ट प्राप्त करता है या सेट करता है। एक कार्य से संबंधित टाइम‑फ़ेज़्ड डेटा ब्लॉक"
type: docs
weight: 1220
url: /hi/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

इस टास्क का TimephasedDataCollection ऑब्जेक्ट प्राप्त करता है या सेट करता है। टास्क से जुड़ा time phased डेटा ब्लॉक।

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## टिप्पणियाँ

पढ़ना केवल XML फ़ॉर्मेट के लिए समर्थित है।

## उदाहरण

दिखाता है कि कार्य के टाइम‑फ़ेज़्ड डेटा पर कैसे इटररेट करें।

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
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


