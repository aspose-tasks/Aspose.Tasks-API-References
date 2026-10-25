---
title: "Resource.Get"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource मेथड। वह मान लौटाता है जिससे यह प्रॉपर्टी इस कंटेनर में मैप की गई है"
type: docs
weight: 830
url: /hi/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह मान लौटाता है।

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | मैप किए गए मान का प्रकार। |
| key | निर्दिष्ट प्रॉपर्टी कुंजी। [`Rsc`](../../rsc/) प्रॉपर्टी कुंजी प्राप्त करने के लिए। |

### रिटर्न वैल्यू

वह मान जिससे यह प्रॉपर्टी इस कंटेनर में मैप की गई है।

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


