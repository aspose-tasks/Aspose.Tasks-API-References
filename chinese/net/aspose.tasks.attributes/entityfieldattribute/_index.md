---
title: "类 EntityFieldAttribute"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Attributes.EntityFieldAttribute 类。表示实体属性的特性"
type: docs
weight: 70
url: /zh/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

表示实体属性的属性。

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | 默认构造函数。 |

## 备注

此特性仅用于 [`Task`](../../aspose.tasks/task/)、[`Resource`](../../aspose.tasks/resource/)、[`Project`](../../aspose.tasks/project/) 和 [`ResourceAssignment`](../../aspose.tasks/resourceassignment/) 实体属性，并简化其枚举。

## 示例

如何使用 **EntityField** 特性枚举属性：

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

### 另见

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


