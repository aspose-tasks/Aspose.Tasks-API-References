---
title: "ExtendedAttributeDefinition.CfType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition प्रॉपर्टी। एक कस्टम फ़ील्ड का प्रकार प्राप्त करता है"
type: docs
weight: 90
url: /hi/net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

कस्टम फ़ील्ड का प्रकार प्राप्त करता है।

```csharp
public CustomFieldType CfType { get; }
```

## उदाहरण

कस्टम विस्तारित एट्रिब्यूट्स के CfType के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// टास्क के लिए विस्तारित एट्रिब्यूट्स पढ़ें
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}
```

### संबंधित देखें

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


