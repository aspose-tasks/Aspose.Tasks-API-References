---
title: "ExtendedAttributeDefinition.FieldId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ExtendedAttributeDefinition. Obtient ou définit l'identifiant du projet d'un champ personnalisé. Utilisez la représentation sous forme de chaîne d'une constante de la classe ExtendedAttributeTask pour spécifier la propriété FieldId"
type: docs
weight: 130
url: /fr/net/aspose.tasks/extendedattributedefinition/fieldid/
---
## ExtendedAttributeDefinition.FieldId property

Obtient ou définit l'identifiant du projet d'un champ personnalisé. Utilisez la représentation sous forme de chaîne d'une constante de la classe [`ExtendedAttributeTask`](../../extendedattributetask/) pour spécifier la propriété `FieldId`.

```csharp
public string FieldId { get; set; }
```

## Remarques

La façon préférable de définir la propriété `FieldId` est de créer [`ExtendedAttributeDefinition`](../) en utilisant l'une des méthodes d'usine dédiées comme [`CreateTaskDefinition`](../createtaskdefinition/) ou [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/).

## Exemples

```csharp
customFieldDefinition.FieldId = Aspose.Tasks.ExtendedAttributeTask.Number10.ToString("D");
```

Montre comment lire les informations communes de la définition d'attribut étendu.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// lire les informations de la définition d'attribut étendu
foreach (var definition in project.ExtendedAttributes)
{
    Console.WriteLine("Guid:" + definition.Guid);
    Console.WriteLine("Secondary Guid:" + definition.SecondaryGuid);
    Console.WriteLine("Secondary Pid:" + definition.SecondaryPid);
    Console.WriteLine("Alias:" + definition.Alias);
    Console.WriteLine("Phonetics Alias:" + definition.PhoneticsAlias);
    Console.WriteLine("Field Id:" + definition.FieldId);
    Console.WriteLine("Project Name:" + definition.ParentProject.Get(Prj.Name));

    Console.WriteLine("Append New Values:" + definition.AppendNewValues);
    Console.WriteLine("Auto RollDown:" + definition.AutoRollDown);
    Console.WriteLine("Calculation Type:" + definition.CalculationType);
    Console.WriteLine("Field Name" + definition.FieldName);
    Console.WriteLine("Is User Defined Custom Field:" + definition.UserDef);
    Console.WriteLine("Rollup Type:" + definition.RollupType);

    if (definition.CalculationType == CalculationType.Lookup)
    {
        Console.WriteLine("  Next properties are used only for lookups:");
        Console.WriteLine("  Default Guid:" + definition.DefaultGuid);
        Console.WriteLine("  Element Type:" + definition.ElementType);
        Console.WriteLine("  Lookup Uid:" + definition.LookupUid);
        Console.WriteLine("  Restrict Values:" + definition.RestrictValues);
        Console.WriteLine("  Max Multi Values:" + definition.MaxMultiValues);
        Console.WriteLine("  Valuelist Sort Order:" + definition.ValuelistSortOrder);
        Console.WriteLine("  Default Value:" + definition.Default);
        Console.WriteLine("  Print values from value list:");
        foreach (var value in definition.ValueList)
        {
            Console.WriteLine("    Description: " + value.Description);
            Console.WriteLine("    Value: " + value.Val);
        }
    }

    Console.WriteLine();
}
```

### Voir aussi

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


