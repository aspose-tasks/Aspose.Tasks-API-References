---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraReadOptions प्रॉपर्टी। कई प्रोजेक्ट्स वाली फ़ाइल से पढ़ने के लिए प्रोजेक्ट का UID प्राप्त करता है या सेट करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

एक फ़ाइल जिसमें कई प्रोजेक्ट हैं, से पढ़ने के लिए प्रोजेक्ट का UID प्राप्त करता है या सेट करता है।

```csharp
public int ProjectUid { get; set; }
```

## उदाहरण

दिखाता है कि कई प्रोजेक्ट्स वाली Primavera XML या Primavera XER फ़ाइल से प्रोजेक्ट कैसे पढ़ें।

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// विशेष UID वाला प्रोजेक्ट लौटाता है।
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


