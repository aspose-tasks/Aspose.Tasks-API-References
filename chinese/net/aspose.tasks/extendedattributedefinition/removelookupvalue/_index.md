---
title: "ExtendedAttributeDefinition.RemoveLookupValue"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttributeDefinition 方法。从内部查找列表中移除一个值。这是操作 ValueList 的首选方式"
type: docs
weight: 340
url: /zh/net/aspose.tasks/extendedattributedefinition/removelookupvalue/
---
## ExtendedAttributeDefinition.RemoveLookupValue method

从内部查找列表中移除一个值。这是操作 [`ValueList`](../valuelist/) 的首选方式。

```csharp
public void RemoveLookupValue(Value value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | 值 | 要从查找中移除的值。 |

## 备注

此方法仅适用于具有 [`CalculationType`](../calculationtype/) 等于 Lookup 的 [`ExtendedAttributeDefinition`](../) 实例。

## 示例

展示如何为分配添加带查找的扩展属性。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 通过创建 ResourceAssignment 对象，将资源 "1 TRG: Trade Group" 分配给 "TASK 1"。
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// 创建带查找的自定义属性定义。
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// 此值可在 MS Project 的 "Resource usage" 视图中看到。
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// 创建带查找的自定义属性定义。
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// 此值可在 MS Project 的 "Task usage" 视图中看到。
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// 错误的值可以稍后删除。
taskCostAttr.RemoveLookupValue(taskWrongValue);

// 正在处理项目...
```

### 另见

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


