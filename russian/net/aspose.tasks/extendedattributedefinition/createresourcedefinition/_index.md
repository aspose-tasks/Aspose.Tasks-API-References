---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ExtendedAttributeDefinition. Фабричный метод, который создаёт простое определение расширенного атрибута, отображаемое в Microsoft Project как None. У него CalculationType равно None и может использоваться только в ресурсах. При вызове этого метода необходимо указать customFieldType, fieldId и alias."
type: docs
weight: 30
url: /ru/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Фабричный метод, который создаёт простое определение расширенного атрибута, отображаемое в Microsoft Project как "None". У него [`CalculationType`](../calculationtype/) равно None и может использоваться только в ресурсах. При вызове этого метода необходимо указать *customFieldType*, *fieldId* и *alias*.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customFieldType | CustomFieldType | Указанный тип [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeResource | Указанный [`ExtendedAttributeResource`](../../extendedattributeresource/) идентификатор поля. |
| alias | Строка | Указанный строковый alias. |

### Возвращаемое значение

Создан экземпляр класса [`ExtendedAttributeDefinition`](../) с указанными *customFieldType*, *fieldId* и *alias*.

## Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Показывает, как добавить расширенный атрибут к назначению ресурса.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Добавить новую задачу и ресурс
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Пользовательские атрибуты, видимые в представлении "Resource Usage", можно создать с помощью метода ExtendedAttributeDefinition.CreateResourceDefinition.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // Тип атрибута — "Cost", поэтому нам нужно использовать свойство "NumericValue".
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Пользовательские атрибуты, видимые в представлении "Task Usage", можно создать с помощью метода ExtendedAttributeDefinition.CreateTaskDefinition.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // Тип атрибута — "Cost", поэтому нам нужно использовать свойство "NumericValue".
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Фабричный метод, который создаёт простое определение расширенного атрибута, отображаемое в Microsoft Project как "None". У него [`CalculationType`](../calculationtype/) равно None и может использоваться только в ресурсах. При вызове этого метода необходимо указать *fieldId* и *alias*. Тип поля выводится из fieldId.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Указанный [`ExtendedAttributeResource`](../../extendedattributeresource/) идентификатор поля. |
| alias | Строка | Указанный строковый alias. |

### Возвращаемое значение

Создан экземпляр класса [`ExtendedAttributeDefinition`](../) с указанными *fieldId* и *alias*.

## Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

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

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


