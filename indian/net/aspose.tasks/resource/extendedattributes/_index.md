---
title: "Resource.ExtendedAttributes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी. विस्तारित एट्रिब्यूट के मान प्राप्त करता है"
type: docs
weight: 320
url: /hi/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

एक विस्तारित विशेषता के मान प्राप्त करता है।

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## टिप्पणियाँ

दो डेटा टुकड़े आवश्यक हैं - विस्तारित एट्रिब्यूट तालिका की ओर एक pointer जो या तो unique ID या Field ID द्वारा निर्दिष्ट किया जाता है, और वह value जो या तो value के साथ निर्दिष्ट किया जाता है, या value list की ओर एक pointer।

## उदाहरण

रिसोर्स विस्तारित एट्रिब्यूट जोड़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// विस्तारित एट्रिब्यूट परिभाषित करें
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// विस्तारित विशेषता बनाएं और उसका मान सेट करें
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// एक नया संसाधन और उसकी विस्तारित विशेषता जोड़ें
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


