---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraReadOptions प्रॉपर्टी। XER फ़ॉर्मेट से पढ़े गए अनिर्दिष्ट बाधाओं वाले कार्यों को प्रोसेस करने के लिए उपयोग किए जाने वाले व्यवहार को निर्दिष्ट करता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

XER फ़ॉर्मेट से पढ़े गए अनिर्धारित प्रतिबंधों वाले टास्क को प्रोसेस करने के लिए उपयोग किए जाने वाले व्यवहार को निर्दिष्ट करता है।

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


