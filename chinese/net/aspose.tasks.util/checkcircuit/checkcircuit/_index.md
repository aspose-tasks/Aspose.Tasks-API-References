---
title: "CheckCircuit.CheckCircuit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CheckCircuit 构造函数。初始化 CheckCircuit 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

初始化 [`CheckCircuit`](../) 类的新实例。

```csharp
public CheckCircuit()
```

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

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


