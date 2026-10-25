---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "LoadOptions प्रॉपर्टी। एन्कोडिंग प्राप्त करता है या सेट करता है जिसका उपयोग HTML MPX XER और Primavera XML फ़ॉर्मैट्स से प्रोजेक्ट पढ़ने के लिए किया जाता है। डिफ़ॉल्ट एन्कोडिंग UTF8 है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए उपयोग की जाने वाली एन्कोडिंग को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट एन्कोडिंग UTF8 है।

```csharp
public Encoding Encoding { get; set; }
```

## उदाहरण

दिखाता है कि Primavera XER फ़ाइल से प्रोजेक्ट खोलते समय एन्कोडिंग कैसे निर्दिष्ट करें।

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### संबंधित देखें

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


