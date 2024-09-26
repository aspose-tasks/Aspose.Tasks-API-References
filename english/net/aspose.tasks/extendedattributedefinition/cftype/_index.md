---
title: ExtendedAttributeDefinition.CfType
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition property. Gets the type of a custom field
type: docs
weight: 90
url: /net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

Gets the type of a custom field.

```csharp
public CustomFieldType CfType { get; }
```

## Examples

Shows how to work with CfType of custom extended attributes.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Read extended attributes for tasks
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

### See Also

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


