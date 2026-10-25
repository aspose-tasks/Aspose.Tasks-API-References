---
title: "ExtendedAttributeDefinition.CfType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttributeDefinition. Επιστρέφει τον τύπο ενός προσαρμοσμένου πεδίου"
type: docs
weight: 90
url: /el/net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

Λαμβάνει τον τύπο ενός προσαρμοσμένου πεδίου.

```csharp
public CustomFieldType CfType { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με CfType των προσαρμοσμένων εκτεταμένων χαρακτηριστικών.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Ανάγνωση εκτεταμένων χαρακτηριστικών για εργασίες
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

### Δείτε επίσης

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


