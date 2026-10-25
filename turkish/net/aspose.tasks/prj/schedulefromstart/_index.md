---
title: "Prj.ScheduleFromStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Proje takvimini başlangıç tarihinden itibaren ileri doğru hesaplayıp hesaplamayacağını belirler"
type: docs
weight: 630
url: /tr/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

Proje takvimini başlangıç tarihinden ileri doğru hesaplayıp hesaplamayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


