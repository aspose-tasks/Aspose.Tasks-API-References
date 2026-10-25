---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "LoadOptions प्रॉपर्टी। PrimaveraReadOptions क्लास की एक निर्दिष्ट इंस्टेंस प्राप्त करता या सेट करता है जिसे Primavera फ़ॉर्मैट्स (Primavera P6 XER या Primavera P6 Xml) लोड करने के व्यवहार को अनुकूलित करने के लिए उपयोग किया जा सकता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

[`PrimaveraReadOptions`](../../primaverareadoptions/) क्लास की एक निर्दिष्ट इंस्टेंस को प्राप्त करता या सेट करता है जिसे Primavera फ़ॉर्मैट्स (Primavera P6 XER या Primavera P6 Xml) लोड करने के व्यवहार को अनुकूलित करने के लिए उपयोग किया जा सकता है।

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
```

## उदाहरण

दिखाता है कि कैसे निर्दिष्ट Id के साथ Primavera प्रोजेक्ट को &lt;see cref="LoadOptions" /&gt; का उपयोग करके लोड किया जाए।

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// Primavera रीडिंग विकल्प सेट करें
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// परियोजना के साथ काम करें...
```

### संबंधित देखें

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


