---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition मेथड। ExtendedAttributeDefinition क्लास के इंस्टेंस के लिए एक हैश कोड लौटाता है।"
type: docs
weight: 330
url: /hi/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

[`ExtendedAttributeDefinition`](../) क्लास के इंस्टेंस के लिए एक हैश कोड लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए एक हैश कोड।

## उदाहरण

दिखाता है कि विस्तारित एट्रिब्यूट परिभाषा का हैश कोड कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// एक विस्तारित एट्रिब्यूट परिभाषा का हैश कोड एक फ़ील्ड आईडी के बराबर है।
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### संबंधित देखें

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


