---
title: "Project.ExtendedAttributes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। ExtendedAttributeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। प्रोजेक्ट से जुड़े विस्तारित एट्रिब्यूट कस्टम फ़ील्ड परिभाषाओं का संग्रह"
type: docs
weight: 410
url: /hi/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

ExtendedAttributeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। यह संग्रह परियोजना से जुड़े विस्तारित विशेषता (कस्टम फ़ील्ड) परिभाषाओं का संग्रह है।

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## उदाहरण

विस्तारित एट्रिब्यूट्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// यदि कस्टम फ़ील्ड प्रोजेक्ट में मौजूद नहीं है, तो इसे बनाएं
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// परिभाषा से विस्तारित एट्रिब्यूट जेनरेट करें
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// टास्क में विस्तारित एट्रिब्यूट जोड़ें
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


