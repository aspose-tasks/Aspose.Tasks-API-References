---
title: "Класс OutlineValueCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.OutlineValueCollection класс. Представляет коллекцию объектов OutlineValue"
type: docs
weight: 1220
url: /ru/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

Представляет коллекцию объектов [`OutlineValue`](../outlinevalue/).

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | Получает значение, указывающее, является ли эта коллекция только для чтения. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | Возвращает или задает элемент по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | Определяет индекс указанного элемента в этой коллекции. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | Вставляет указанный элемент в указанный индекс. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | Удаляет элемент по указанному индексу. |

## Примеры

Показывает, как работать с коллекциями значений контуров.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// очистить коллекции значений
foreach (var outlineCode in project.OutlineCodes)
{
    // очистить маски контуров
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// обновить значение по индексу доступа
codeDefinition.Values[0].Value = "654321";

// итерация по значениям контуров
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// работа с значениями контуров
// ...

// удалить значение при необходимости
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// вставить значение в начальную позицию
codeDefinition.Values.Insert(0, value);

// проверить позицию вставленного значения
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// работа с значениями контуров
// ...

// удалить последнее значение из коллекции
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// можно создать другое определение кода контура
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// а затем скопировать значения контуров
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### См. также

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


