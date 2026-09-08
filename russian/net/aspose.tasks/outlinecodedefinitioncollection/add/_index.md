---
title: "OutlineCodeDefinitionCollection.Add"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод OutlineCodeDefinitionCollection. Добавляет указанный элемент в эту коллекцию."
type: docs
weight: 40
url: /ru/net/aspose.tasks/outlinecodedefinitioncollection/add/
---
## OutlineCodeDefinitionCollection.Add method

Добавляет указанный элемент в эту коллекцию.

```csharp
public void Add(OutlineCodeDefinition item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | OutlineCodeDefinition | указанный элемент для добавления в эту коллекцию. |

## Примеры

Показывает, как работать с коллекциями определений контурного кода.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// добавьте пользовательское определение outline code
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // вставить определение контурного кода в позицию
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// найти индекс определения контурного кода
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// редактировать определение кода структуры
project.OutlineCodes[index].Alias = "New Alias";

// ...
// работать с определениями кода структуры
// ...

// удалить определение кода структуры
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// удалить определение кода структуры по индексу
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// удалить определения кода структуры
otherProject.OutlineCodes.Clear();

// скопировать определения кода структуры
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// работать с определениями кода структуры
// ...

// удалять определения кода структуры по одному
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### См. также

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


