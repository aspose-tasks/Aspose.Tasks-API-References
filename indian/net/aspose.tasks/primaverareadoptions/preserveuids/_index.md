---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraReadOptions प्रॉपर्टी। एक फ़्लैग प्राप्त करता है या सेट करता है जो यह निर्धारित करता है कि इकाइयों के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

एक फ़्लैग प्राप्त करता है या सेट करता है जो यह निर्दिष्ट करता है कि इकाइयों के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं।

```csharp
public bool PreserveUids { get; set; }
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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


