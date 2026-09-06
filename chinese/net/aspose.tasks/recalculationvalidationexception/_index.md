---
title: "类 RecalculationValidationException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RecalculationValidationException 类。表示在重新计算后项目中发现错误时抛出的异常"
type: docs
weight: 1680
url: /zh/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

表示在重新计算后发现项目错误而抛出的异常。

```csharp
public abstract class RecalculationValidationException : ValidationException
```

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

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


