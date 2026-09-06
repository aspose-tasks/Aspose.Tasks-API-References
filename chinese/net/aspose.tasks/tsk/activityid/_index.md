---
title: "Tsk.ActivityId"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。表示活动 ID 字段，即 Primavera 使用的任务唯一标识符。仅适用于 Primavera 项目"
type: docs
weight: 10
url: /zh/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

表示活动 ID 字段——Primavera 使用的任务唯一标识符。（仅适用于 Primavera 项目）

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## 示例

展示如何使用 Primavera 项目特定的 ActivityId 字段

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// 创建 Primavera 保存选项并指定在保存期间不应覆盖 ActivityIds。
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


