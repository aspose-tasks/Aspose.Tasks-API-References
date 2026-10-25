---
title: "ExtendedAttributeDefinition.CfType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttributeDefinition. تحصل على نوع الحقل المخصص"
type: docs
weight: 90
url: /ar/net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

يحصل على نوع الحقل المخصص.

```csharp
public CustomFieldType CfType { get; }
```

## الأمثلة

يعرض كيفية العمل مع CfType للسمات الموسعة المخصصة.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// قراءة السمات الموسعة للمهام
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

### انظر أيضًا

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


