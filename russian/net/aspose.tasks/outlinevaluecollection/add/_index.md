---
title: "OutlineValueCollection.Add"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод OutlineValueCollection. Добавляет указанный элемент в эту коллекцию"
type: docs
weight: 40
url: /ru/net/aspose.tasks/outlinevaluecollection/add/
---
## OutlineValueCollection.Add method

Добавляет указанный элемент в эту коллекцию.

```csharp
public void Add(OutlineValue item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | OutlineValue | указанный элемент для добавления в эту коллекцию. |

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

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


