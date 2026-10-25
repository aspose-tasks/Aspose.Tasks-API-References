---
title: "ExtendedAttributeDefinition.FieldId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttributeDefinition. Возвращает или задает значение, соответствующее идентификатору проекта пользовательского поля. Используйте строковое представление константы из класса ExtendedAttributeTask для указания свойства FieldId"
type: docs
weight: 130
url: /ru/net/aspose.tasks/extendedattributedefinition/fieldid/
---
## ExtendedAttributeDefinition.FieldId property

Возвращает или задает значение, соответствующее идентификатору проекта пользовательского поля. Используйте строковое представление константы из класса [`ExtendedAttributeTask`](../../extendedattributetask/) для указания свойства `FieldId`.

```csharp
public string FieldId { get; set; }
```

## Примечания

Предпочтительный способ установить свойство `FieldId` — создать [`ExtendedAttributeDefinition`](../), используя один из специализированных фабричных методов, таких как [`CreateTaskDefinition`](../createtaskdefinition/) или [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/).

## Примеры

```csharp
customFieldDefinition.FieldId = Aspose.Tasks.ExtendedAttributeTask.Number10.ToString("D");
```

Показывает, как прочитать общую информацию определения расширенного атрибута.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// читать информацию определения расширенного атрибута
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

### См. также

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


