---
title: "类 TaskValidationException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskValidationException 类。表示在重新计算后发现项目任务错误时抛出的异常"
type: docs
weight: 2510
url: /zh/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

表示在重新计算后发现项目任务错误时抛出的异常。

```csharp
public class TaskValidationException : RecalculationValidationException
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | 获取导致异常的任务。 |

## 示例

显示在什么条件下可以抛出 &lt;see cref=\"TaskValidationException\" /&gt; 异常。

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // 意外设置了不正确的日期
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // 使用标志运行项目重新计算以执行验证
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


