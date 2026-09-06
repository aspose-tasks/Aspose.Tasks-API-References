---
title: "CheckCircuit.Alg"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CheckCircuit 方法。检查指定的对象是否已经被处理"
type: docs
weight: 20
url: /zh/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

检查指定的对象是否已被处理。

```csharp
public override void Alg(Task el, int level)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | 任务 | 要处理的对象。 |
| 级别 | Int32 | 树节点层级。 |

## 示例

展示如何检测损坏的项目结构。

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// 检查项目结构。
// 如果项目结构不正确，将抛出 <see cref=\"TasksException\">。
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### 另见

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


