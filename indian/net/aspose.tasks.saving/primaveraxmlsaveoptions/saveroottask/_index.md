---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraXmlSaveOptions प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि रूट टास्क को सहेजना है या नहीं"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि रूट टास्क को सहेजा जाए या नहीं।

```csharp
public bool SaveRootTask { get; set; }
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


