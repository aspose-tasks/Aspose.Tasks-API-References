---
title: "Sınıf TaskValidationException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskValidationException sınıfı. Yeniden hesaplamadan sonra proje görevlerinde hatalar bulunduğunda atılan bir istisna temsil eder"
type: docs
weight: 2510
url: /tr/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

Yeniden hesaplamadan sonra projenin görevlerinde hatalar bulunduğunda fırlatılan bir istisnayı temsil eder.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | İstisnaya neden olan görevi alır. |

## Örnekler

Hangi koşullarda &lt;see cref=\"TaskValidationException\" /&gt; istisnasının atılabileceğini gösterir.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // yanlışlıkla hatalı tarihleri ayarla
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // doğrulamayı çalıştırmak için bir bayrakla proje yeniden hesaplamasını çalıştır
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ayrıca Bakınız

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


