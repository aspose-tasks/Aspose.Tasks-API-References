---
title: "Class RecalculationValidationException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RecalculationValidationException sınıfı. Yeniden hesaplamadan sonra projede hatalar bulunduğunda atılan bir istisna temsil eder."
type: docs
weight: 1680
url: /tr/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

Proje yeniden hesaplandıktan sonra hatalar bulunduğunda atılan bir istisna temsil eder.

```csharp
public abstract class RecalculationValidationException : ValidationException
```

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

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


