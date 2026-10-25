---
title: "TreeAlgorithmBase1.PreAlg"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TreeAlgorithmBase 方法。在处理树节点之前调用。"
type: docs
weight: 30
url: /zh/net/aspose.tasks.util/treealgorithmbase-1/prealg/
---
## TreeAlgorithmBase&lt;T&gt;.PreAlg method

在处理树的节点之前调用。

```csharp
public virtual void PreAlg(T el, int level)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要处理的节点。 |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


