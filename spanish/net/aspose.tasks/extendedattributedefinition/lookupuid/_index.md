---
title: "ExtendedAttributeDefinition.LookupUid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ExtendedAttributeDefinition. Obtiene un Guid de la tabla de búsqueda asociada a un campo personalizado"
type: docs
weight: 180
url: /es/net/aspose.tasks/extendedattributedefinition/lookupuid/
---
## ExtendedAttributeDefinition.LookupUid property

Obtiene un GUID de la tabla de búsqueda asociada a un campo personalizado.

```csharp
public string LookupUid { get; }
```

## Observaciones

Para crear un campo personalizado con búsqueda, use uno de los métodos de fábrica: [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/) o [`CreateLookupResourceDefinition`](../createlookupresourcedefinition/).

## Ejemplos

Muestra cómo leer la información común de la definición de atributo extendido.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// leer información de la definición de atributo extendido
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

### Ver también

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


