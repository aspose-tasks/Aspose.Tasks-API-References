---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraXmlSaveOptions कंस्ट्रक्टर। PrimaveraXmlSaveOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

[`PrimaveraXmlSaveOptions`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public PrimaveraXmlSaveOptions()
```

## उदाहरण

दिखाता है कि Primavera XML फ़ाइल में कैसे निर्यात किया जाए।

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### संबंधित देखें

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


