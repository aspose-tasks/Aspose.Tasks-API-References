---
title: "Enum CalculationMode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CalculationMode enum. Proje hesaplama modunu belirtir"
type: docs
weight: 210
url: /tr/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

Proje hesaplama modunu belirtir.

```csharp
public enum CalculationMode
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | None. Proje tarihleri ve maliyetleri bu modda yeniden hesaplanmaz. |
| Automatic | `1` | Automatic mode. Bu mod kullanıldığında proje tarihleri ve maliyetleri yeniden hesaplanır. |
| Manual | `2` | Manual mode. Bu modda yalnızca gerekli alanlar yeniden hesaplanır, örneğin nesnelerin UID ve ID'leri. |

## Örnekler

Auto calculation mode'un nasıl kullanılacağını gösterir.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// Proje başlangıç tarihini ayarlayın ve yeni görevler ekleyin
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Görevleri bağlayın
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Tarihlerin yeniden hesaplandığını doğrulayın
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

None calculation mode'un nasıl kullanılacağını gösterir.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// Yeni bir görev ekleyin
var task = project.RootTask.Children.Add("Task");

// Not: kimlikler bile hesaplanmadı
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// Süre özelliğini ayarlayın
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

Manual calculation mode'un nasıl kullanılacağını gösterir.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Proje başlangıç tarihini ayarlayın ve yeni görevler ekleyin
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Gerekli özellikler manual modda ayarlanır
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// İki görevi birleştirdiğimizde, tarihleri manual modda yeniden hesaplanmaz
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Görev 2 Başlangıcı değişmedi
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


