---
title: "类 TasksReadingException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TasksReadingException 类。表示标准内部读取异常类型"
type: docs
weight: 2540
url: /zh/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

表示标准内部读取异常类型。

```csharp
public class TasksReadingException : TasksLoggedException
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | 获取异常日志信息。 |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | 获取异常操作信息。 |

## 示例

展示如何处理项目的读取/写入异常。

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### 另见

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


