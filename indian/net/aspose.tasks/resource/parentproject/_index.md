---
title: "Resource.ParentProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी. इस कंटेनर के लिए पैरेंट प्रोजेक्ट प्राप्त करता है"
type: docs
weight: 600
url: /hi/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

प्राप्त करता है इस कंटेनर के लिए पैरेंट प्रोजेक्ट।

```csharp
public Project ParentProject { get; }
```

## उदाहरण

रिसोर्स के पैरेंट प्रोजेक्ट का उपयोग कैसे करें दिखाता है।

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// डिफ़ॉल्ट प्रोजेक्ट कार्य समय इकाई प्रकार का उपयोग करके रिसोर्स के लिए कार्य सेट करें।
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### संबंधित देखें

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


