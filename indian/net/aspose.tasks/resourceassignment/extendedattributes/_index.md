---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment प्रॉपर्टी। इस ऑब्जेक्ट के लिए ExtendedAttributeCollection क्लास का एक इंस्टेंस प्राप्त करता है या सेट करता है"
type: docs
weight: 250
url: /hi/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

इस ऑब्जेक्ट के लिए ExtendedAttributeCollection क्लास का एक इंस्टेंस प्राप्त करता है या सेट करता है।

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## टिप्पणियाँ

पढ़ना केवल XML फ़ॉर्मेट के लिए समर्थित है।

## उदाहरण

दिखाता है कि कैसे एक असाइनमेंट के लिए विस्तारित विशेषताएँ जोड़ी जाएँ।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// एक ResourceAssignment ऑब्जेक्ट बनाकर संसाधन "1 TRG: Trade Group" को "TASK 1" को असाइन करें।
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// लुकअप के साथ कस्टम एट्रिब्यूट परिभाषा बनाएं।
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// यह मान MS Project के "Resource usage" दृश्य में देखा जा सकता है।
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### संबंधित देखें

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


