---
title: "ExtendedAttribute.IsErrorValue"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttribute. Возвращает, произошла ли ошибка при вычислении значения расширенных атрибутов"
type: docs
weight: 60
url: /ru/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

Определяет, привела ли вычисление значения расширенного атрибута к ошибке.

```csharp
public bool IsErrorValue { get; }
```

## Примеры

Показывает, как добавить пользовательское поле, значение которого рассчитывается с помощью формулы, указанной пользователем.

```csharp
var project = new Project();

// создать новое определение расширенного атрибута задачи
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Добавьте формулу к атрибуту.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Создать расширенный атрибут
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Мы задаем Формулу для расширенного атрибута, поэтому он только для чтения (значение рассчитывается с помощью формулы).
// Вывод: "Значение только для чтения"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Вы можете попытаться установить значение только для чтения поля, но это не даст эффекта.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### См. также

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


