---
title: "类 OutlineCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OutlineCode 类。表示大纲代码的一个值"
type: docs
weight: 1150
url: /zh/net/aspose.tasks/outlinecode/
---
## OutlineCode class

表示大纲代码的值。

```csharp
public class OutlineCode
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | 初始化 `OutlineCode` 类的新实例。 |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | 使用指定的大纲代码及其其中一个值来初始化 `OutlineCode` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | 获取或设置项目 Id 自定义字段的数值。 |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | 获取或设置值列表中值的 GUID。ValueGuid 与值列表中的 FieldGuid 相匹配。 |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | 获取或设置值列表中与大纲代码集合定义关联的 Id。 |

## 备注

需要两条数据——由 FieldId 指定的大纲代码表指针，以及通过 ValueId 或 ValueGuid（指向值列表的指针）指定的值。

## 示例

展示如何读取任务的大纲代码。

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// 读取大纲代码
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


