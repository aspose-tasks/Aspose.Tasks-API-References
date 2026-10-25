---
title: "Calendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Görevin bitiş tarih ve saatini, başlangıç tarihinin bölünmüş parçalarından ve iş süresinden hesaplar"
type: docs
weight: 210
url: /tr/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Görevin başlangıç tarihi, bölünmüş parçaları ve çalışma süresinden görev bitiş tarih ve saatini hesaplar.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Bitiş tarihini hesaplamak için görev. |
| süre | TimeSpan | Hesaplanacak süre. |

### Dönüş Değeri

Verilen başlangıç tarihi ve süre için görevin bitiş tarihi.

## Açıklamalar

Görev özet ise, null ise veya başlangıç tarihi ayarlanmamışsa DateTime.MinValue döndürür.

## Örnekler

Özel bir süre kullanarak bir görevin bitiş tarihinin nasıl hesaplanacağını gösterir.

```csharp
var project = new Project(DataDir + "SplitTaskFinishDate.mpp");

// Bölünmüş bir görevi bulun
var task = project.RootTask.Children.GetByUid(4);

// Proje takvimini bulun
var calendar = project.Get(Prj.Calendar);

// Görevin bitiş tarihini farklı sürelerle hesaplayın
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 8 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(8, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 16 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(16, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 24 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(24, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 28 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(28, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 32 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(32, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 46 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(46, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 61 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(61, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 75 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(75, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 80 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(80, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 120 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(120, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 150 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(150, 0, 0)));
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


