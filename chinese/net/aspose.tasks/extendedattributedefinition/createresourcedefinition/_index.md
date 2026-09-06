---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttributeDefinition 方法。工厂方法，用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 None。其 CalculationType 为 None，仅可在 Resource 中使用。调用此方法时必须指定 customFieldType、fieldId 和 alias。"
type: docs
weight: 30
url: /zh/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

工厂方法，用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 "None"。它的 [`CalculationType`](../calculationtype/) 为 None，仅可在 Resource 中使用。调用此方法时必须指定 *customFieldType*、*fieldId* 和 *alias*。

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| customFieldType | CustomFieldType | 指定的 [`CustomFieldType`](../../customfieldtype/) 类型。 |
| fieldId | ExtendedAttributeResource | 指定的 [`ExtendedAttributeResource`](../../extendedattributeresource/) 字段 ID。 |
| 别名 | 字符串 | 指定的 String 别名。 |

### 返回值

已创建带有指定 *customFieldType*、*fieldId* 和 *alias* 的 [`ExtendedAttributeDefinition`](../) 类实例。

## 示例

使用此示例创建自定义文本字段定义：

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

展示如何向资源分配添加扩展属性。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 添加新任务和资源
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // 在 "Resource Usage" 视图中可见的自定义属性可以使用 ExtendedAttributeDefinition.CreateResourceDefinition 方法创建。
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // 属性的类型是 "Cost"，因此我们需要使用 "NumericValue" 属性。
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // 在 "Task Usage" 视图中可见的自定义属性可以使用 ExtendedAttributeDefinition.CreateTaskDefinition 方法创建。
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // 属性的类型是 "Cost"，因此我们需要使用 "NumericValue" 属性。
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

工厂方法，用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 "None"。它的 [`CalculationType`](../calculationtype/) 为 None，仅可在 Resource 中使用。调用此方法时必须指定 *fieldId* 和 *alias*。字段类型将根据 fieldId 推断。

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | 指定的 [`ExtendedAttributeResource`](../../extendedattributeresource/) 字段 ID。 |
| 别名 | 字符串 | 指定的 String 别名。 |

### 返回值

已创建带有指定 *fieldId* 和 *alias* 的 [`ExtendedAttributeDefinition`](../) 类实例。

## 示例

使用此示例创建自定义文本字段定义：

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

展示如何创建扩展属性定义并在构建时设置标志的值。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// 为布尔自定义字段创建定义
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// 创建属性并将初始值设为 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### 另见

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


