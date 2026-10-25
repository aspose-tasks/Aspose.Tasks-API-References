---
title: "类 TasksWritingException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TasksWritingException 类。表示标准内部写入异常类型"
type: docs
weight: 2560
url: /zh/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

表示标准内部写入异常类型。

```csharp
public class TasksWritingException : TasksLoggedException
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | 获取异常日志信息。 |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | 获取异常操作信息。 |

## 示例

展示如何读取日志文本和异常类型以检查 MPP 导出的问题。

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // 将项目导出为 MPP 文件
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### 另见

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


