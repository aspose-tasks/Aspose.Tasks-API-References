---
title: "ExtendedAttributeDefinition.CfType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ExtendedAttributeDefinition. Mendapatkan tipe bidang khusus"
type: docs
weight: 90
url: /id/net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

Mendapatkan tipe dari bidang khusus.

```csharp
public CustomFieldType CfType { get; }
```

## Contoh

Menunjukkan cara bekerja dengan CfType dari atribut ekstended khusus.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Baca atribut ekstended untuk tugas
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

### Lihat Juga

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


