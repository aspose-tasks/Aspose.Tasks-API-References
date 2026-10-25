---
title: "类 ValidationException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ValidationException 类。表示在实体验证期间发现错误时抛出的异常。"
type: docs
weight: 2790
url: /zh/net/aspose.tasks/validationexception/
---
## ValidationException class

表示在实体验证期间发现错误时抛出的异常。

```csharp
public class ValidationException : ApplicationException
```

## 示例

展示如何在处理循环任务时处理 &lt;see cref=\"ValidationException\"/&gt;。

```csharp
try
{
    var project = new Project();
    var parameters = new RecurringTaskParameters { TaskName = "t1", Duration = project.GetDuration(1, TimeUnitType.Day), RecurrencePattern = null };
    project.RootTask.Children.Add(parameters);
}
catch (ValidationException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


