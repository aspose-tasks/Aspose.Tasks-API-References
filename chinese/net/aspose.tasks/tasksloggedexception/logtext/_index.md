---
title: "TasksLoggedException.LogText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TasksLoggedException 属性。获取异常日志信息。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/tasksloggedexception/logtext/
---
## TasksLoggedException.LogText property

获取异常日志信息。

```csharp
public string LogText { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


