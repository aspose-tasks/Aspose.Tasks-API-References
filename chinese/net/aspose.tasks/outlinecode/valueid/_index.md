---
title: "OutlineCode.ValueId"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineCode 属性。获取或设置值列表中与大纲代码集合定义关联的 Id。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/outlinecode/valueid/
---
## OutlineCode.ValueId property

获取或设置值列表中与大纲代码集合定义关联的 Id。

```csharp
public int ValueId { get; set; }
```

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

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


