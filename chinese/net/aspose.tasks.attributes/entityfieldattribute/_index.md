---
title: Class EntityFieldAttribute
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.Attributes.EntityFieldAttribute 班级. 表示实体属性的属性
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

| 姓名 | 描述 |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | 默认构造函数。 |

### 评论

属性用于[`Task`](../../aspose.tasks/task/),[`Resource`](../../aspose.tasks/resource/),[`Project`](../../aspose.tasks/project/) 和[`ResourceAssignment`](../../aspose.tasks/resourceassignment/)仅限实体属性，并简化其枚举。

### 例子

如何枚举属性使用 **实体字段**属性：

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

### 也可以看看

* 命名空间 [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* 部件 [Aspose.Tasks](../../)


