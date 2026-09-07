---
title: "ExtendedAttribute.ToString"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttribute मेथड। विस्तारित एट्रिब्यूट का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है।"
type: docs
weight: 110
url: /hi/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

विस्तारित गुण का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है।

```csharp
public override string ToString()
```

### रिटर्न वैल्यू

विस्तारित एट्रिब्यूट का स्ट्रिंग प्रतिनिधित्व।

## उदाहरण

विस्तारित एट्रिब्यूट पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// टास्क के लिए विस्तारित एट्रिब्यूट्स पढ़ें
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // विस्तारित एट्रिब्यूट के सामान्य जानकारी पढ़ें
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### संबंधित देखें

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


