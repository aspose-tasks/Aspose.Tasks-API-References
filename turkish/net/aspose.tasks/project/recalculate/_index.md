---
title: "Project.Recalculate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Tüm proje görevlerinin ids, outline levels, start/finish dates, early/late dates ayarlar, slacks, work ve cost fields hesaplar."
type: docs
weight: 1150
url: /tr/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar.

```csharp
public void Recalculate()
```

## Örnekler

Projeyi bitiş tarihinden değil başlangıç tarihinden yeniden planlamanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Şimdi tüm görev tarihleri (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) hesaplanıyor. Kritik yolu elde etmek için gecikmeleri (slack) hesaplamamız gerekir (ayrı bir iş parçacığında çağrılabilir, ancak tüm erken/geç tarihlerin hesaplanmasından sonra).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

İsteğe bağlı doğrulama ile tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar.

```csharp
public void Recalculate(bool validate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| validate | Boolean | Doğru ise yeniden hesaplama doğrulaması yapılır. Hangi verilerin doğrulandığı: Şu anda yalnızca görev ve görev bağlantısı tarih aralıklarının temel doğrulaması uygulanmaktadır. Görev tarih aralıkları (örn. ActualStart - ActualFinish, EarlyStart - EarlyFinish, vb.) ve Görev Bağlantıları tarihleri, başlangıç tarihinin bitiş tarihinden küçük veya eşit olduğu kriterine göre kontrol edilecektir. Yukarıda açıklanan koşullardan herhangi biri başarısız olursa [`RecalculationValidationException`](../../recalculationvalidationexception/) fırlatılır. |

## Örnekler

Projeyi son doğrulama ile yeniden hesaplamanın nasıl yapılacağını gösterir.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // Projeyi son doğrulama ile yeniden hesapla
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


