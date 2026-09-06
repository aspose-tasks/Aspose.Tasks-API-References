---
title: "类 CheckCircuit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.CheckCircuit 类。检查任务树是否包含回路"
type: docs
weight: 2680
url: /zh/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

检查任务树是否包含回路。

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | 初始化 `CheckCircuit` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | 检查指定的对象是否已被处理。 |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


