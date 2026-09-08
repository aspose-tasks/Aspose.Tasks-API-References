---
title: "Класс OutlineCodeDefinitionCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.OutlineCodeDefinitionCollection. Представляет коллекцию объектов OutlineCodeDefinition."
type: docs
weight: 1180
url: /ru/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

Представляет коллекцию объектов [`OutlineCodeDefinition`](../outlinecodedefinition/).

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Возвращает или задает элемент по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Определяет индекс указанного элемента в этой коллекции. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Вставляет указанный элемент в указанный индекс. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Удаляет элемент по указанному индексу. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Преобразует объект OutlineCodeDefinitionCollection в список объектов [`OutlineCodeDefinition`](../outlinecodedefinition/). |

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

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


