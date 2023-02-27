---
title: Class EntityFieldAttribute
second_title: Aspose.Tasks för .NET API-referens
description: Aspose.Tasks.Attributes.EntityFieldAttribute klass. Representerar ett attribut för entitetsegenskaper.
type: docs
weight: 70
url: /sv/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Representerar ett attribut för entitetsegenskaper.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Default_Constructor |

### Anmärkningar

Attribut används för[`Task`](../../aspose.tasks/task/) ,[`Resource`](../../aspose.tasks/resource/) ,[`Project`](../../aspose.tasks/project/) och[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) endast entitetsegenskaper och förenklar dess uppräkning.

### Exempel

Hur man räknar upp egenskaper med hjälp av **EntityField** attribut:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### Se även

* namnutrymme [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* hopsättning [Aspose.Tasks](../../)


