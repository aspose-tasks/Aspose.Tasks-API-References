---
title: "ExtendedAttributeDefinition.CfType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ExtendedAttributeDefinition. Obtient le type d'un champ personnalisé"
type: docs
weight: 90
url: /fr/net/aspose.tasks/extendedattributedefinition/cftype/
---
## ExtendedAttributeDefinition.CfType property

Obtient le type d’un champ personnalisé.

```csharp
public CustomFieldType CfType { get; }
```

## Exemples

Montre comment travailler avec CfType des attributs étendus personnalisés.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Lire les attributs étendus pour les tâches
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

### Voir aussi

* enum [CustomFieldType](../../customfieldtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


