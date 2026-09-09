---
title: "ExtendedAttributeDefinition.CfType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition özelliği. Özel bir alanın türünü alır"
type: docs
weight: 90
url: /tr/net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

Özel bir alanın türünü alır.

```csharp
public CustomFieldType CfType { get; }
```

## Örnekler

Özel genişletilmiş özniteliklerin CfType'ı ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Görevler için genişletilmiş öznitelikleri okuyun
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

### Ayrıca Bakınız

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


