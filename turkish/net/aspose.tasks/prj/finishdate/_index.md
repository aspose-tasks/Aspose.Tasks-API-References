---
title: "Prj.FinishDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin bitiş tarihi"
type: docs
weight: 330
url: /tr/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

Bir projenin bitiş tarihi.

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
```

## Örnekler

Projenin başlangıç tarihinden ziyade bitiş tarihinden yeniden planlanmasının nasıl yapılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Şimdi tüm görev tarihleri (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) hesaplanıyor. Kritik yolu elde etmek için gecikmeleri (slack) hesaplamamız gerekir (ayrı bir iş parçacığında çağrılabilir, ancak tüm erken/geç tarihlerin hesaplanmasından sonra).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


