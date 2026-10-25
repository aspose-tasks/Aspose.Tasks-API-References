---
title: "Project.Get"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह मान लौटाता है"
type: docs
weight: 1080
url: /hi/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह मान लौटाता है।

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | मैप किए गए मान का प्रकार। |
| key | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [`Prj`](../../prj/) |

### रिटर्न वैल्यू

वह मान जिससे यह प्रॉपर्टी इस कंटेनर में मैप की गई है।

## उदाहरण

दिखाता है कि प्रोजेक्ट संस्करण कैसे जांचें।

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// प्रोजेक्ट संस्करण दिखाएँ
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


