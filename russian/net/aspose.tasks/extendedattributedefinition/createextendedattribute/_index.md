---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ExtendedAttributeDefinition. Создаёт новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта"
type: docs
weight: 310
url: /ru/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Возвращаемое значение

возвращает созданный экземпляр класса [`ExtendedAttribute`](../../extendedattribute/) с fieldID, равным значению fieldID этого объекта.

## Примеры

Показывает, как создавать расширенные атрибуты.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Если пользовательское поле не существует в проекте, создайте его
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Создать расширенный атрибут из определения
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Добавить расширенный атрибут к задаче
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным текстовым значением.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| textValue | Строка | Указанное текстовое значение. |

### Возвращаемое значение

возвращает созданный экземпляр класса [`ExtendedAttribute`](../../extendedattribute/) с fieldID, равным значению fieldID этого объекта.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Если текущий [`CfType`](../cftype/) не равен 'Text' |

## Примеры

Показывает, как создать определение расширенного атрибута и установить строковое значение атрибута во время его создания.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// создать расширенный атрибут со значением, равным 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// добавить расширенный атрибут, инициализированный значением 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### См. также

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным числовым значением.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| numericValue | Decimal | Указанное числовое значение. |

### Возвращаемое значение

возвращает созданный экземпляр класса [`ExtendedAttribute`](../../extendedattribute/) с fieldID, равным значению fieldID этого объекта.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Если текущий [`CfType`](../cftype/) не равен 'Number' или 'Cost' |

## Примеры

Показывает, как создать определение расширенного атрибута и установить десятичное значение атрибута во время его создания.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// создать расширенный атрибут со значением, равным 999m
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// добавить расширенный атрибут, инициализированный значением 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### См. также

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением даты.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dateTimeValue | DateTime | Указанное значение даты и времени. |

### Возвращаемое значение

возвращает созданный экземпляр класса [`ExtendedAttribute`](../../extendedattribute/) с fieldID, равным значению fieldID этого объекта.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Если текущий [`CfType`](../cftype/) не является 'Date', 'Start' или 'Finish' |

## Примеры

Показывает, как создать определение расширенного атрибута и установить значение даты и времени атрибута во время его создания.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// создать расширенный атрибут со значением, равным DateTime.Now 
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// добавить расширенный атрибут
task.ExtendedAttributes.Add(extendedAttribute);
```

### См. также

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением длительности.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| durationValue | Продолжительность | Указанное значение длительности. |

### Возвращаемое значение

возвращает созданный экземпляр класса [`ExtendedAttribute`](../../extendedattribute/) с fieldID, равным значению fieldID этого объекта.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Если текущий [`CfType`](../cftype/) не является 'Duration' |

## Примеры

Показывает, как создать определение расширенного атрибута и установить длительность во время его создания.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// расширенный атрибут Duration1 = 2 дня
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// добавить расширенный атрибут к задаче
task.ExtendedAttributes.Add(extendedAttribute);
```

### См. также

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением флага.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| flagValue | Boolean | Указанное значение флага. |

### Возвращаемое значение

возвращает созданный экземпляр класса [`ExtendedAttribute`](../../extendedattribute/) с fieldID, равным значению fieldID этого объекта.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Если текущий [`CfType`](../cftype/) не является 'Flag' |

## Примеры

Показывает, как создать определение расширенного атрибута и установить значение флага во время его создания.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// создать определение для логического пользовательского поля
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// создать атрибут и установить начальное значение 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### См. также

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Создаёт новый расширенный атрибут, связанный с указанным элементом [`Value`](../../value/).

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| lookupValue | Value | Указанный элемент [`Value`](../../value/). |

### Возвращаемое значение

возвращает созданный экземпляр класса [`ExtendedAttribute`](../../extendedattribute/), связанный с указанным элементом [`Value`](../../value/).

## Примечания

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Примеры

Используйте этот код для создания нового [`ExtendedAttribute`](../../extendedattribute/) с использованием конкретного значения:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Показывает, как создать определение расширенного атрибута и установить значение во время его создания.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Создайте определение пользовательского поля на основе таблицы поиска, объявленной выше.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// создать расширенный атрибут для значения 
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// добавить расширенный атрибут к задаче
task.ExtendedAttributes.Add(extendedAttribute);
```

### См. также

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


