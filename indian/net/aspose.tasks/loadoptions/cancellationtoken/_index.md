---
title: "LoadOptions.CancellationToken"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "LoadOptions प्रॉपर्टी। एक टोकन प्राप्त करता है या सेट करता है जिसका उपयोग प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए उपयोग किए जा सकने वाले टोकन को प्राप्त करता है या सेट करता है।

```csharp
public CancellationToken CancellationToken { get; set; }
```

## उदाहरण

दिखाता है कि लम्बे समय तक चलने वाले प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए CancellationToken कैसे पास करें।

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts को किसी अन्य थ्रेड में पास किया जा सकता है जहाँ मेथड cts.Cancel() को कॉल करके प्रोजेक्ट लोडिंग ऑपरेशन को रद्द किया जा सकता है।
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### संबंधित देखें

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


