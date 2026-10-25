---
title: "ExtendedAttributeDefinition.CfType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttributeDefinition. Restituisce il tipo di un campo personalizzato"
type: docs
weight: 90
url: /it/net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

Ottiene il tipo di un campo personalizzato.

```csharp
public CustomFieldType CfType { get; }
```

## Esempi

Mostra come lavorare con CfType di attributi estesi personalizzati.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Leggi gli attributi estesi per i task
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

### Vedi anche

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


