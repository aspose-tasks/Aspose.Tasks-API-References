---
title: "Resource.Set"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource मेथड। इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान से मैप करता है"
type: docs
weight: 860
url: /hi/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | मैप किए गए मान का प्रकार। |
| key | निर्दिष्ट प्रॉपर्टी कुंजी। [`Rsc`](../../rsc/) प्रॉपर्टी कुंजी प्राप्त करने के लिए। |
| मान | मान। |

## उदाहरण

सामान्य रिसोर्स प्रॉपर्टीज़ को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// रिसोर्स जोड़ें और कुछ प्रॉपर्टीज़ सेट करें
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | Key`2 | निर्दिष्ट प्रॉपर्टी कुंजी। [`Rsc`](../../rsc/) प्रॉपर्टी कुंजी प्राप्त करने के लिए। |
| मान | DateTime | मान। |

## उदाहरण

सामान्य रिसोर्स प्रॉपर्टीज़ को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// रिसोर्स जोड़ें और कुछ प्रॉपर्टीज़ सेट करें
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


