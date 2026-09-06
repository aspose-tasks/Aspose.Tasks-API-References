---
title: "类 TasksException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TasksException 类。表示标准内部异常类型。"
type: docs
weight: 2520
url: /zh/net/aspose.tasks/tasksexception/
---
## TasksException class

表示标准内部异常类型。

```csharp
public class TasksException : ApplicationException
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


