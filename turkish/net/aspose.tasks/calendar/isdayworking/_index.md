---
title: "Calendar.IsDayWorking"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Belirtilen günün takvime göre çalışma günü olup olmadığını belirler."
type: docs
weight: 260
url: /tr/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Belirtilen günün takvime göre bir çalışma günü olup olmadığını belirler.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | DateTime | Günün çalışıp çalışmadığını kontrol etmek için tarih. |

### Dönüş Değeri

Gün bir çalışma günü ise doğru.

## Örnekler

Çalışma saatlerini nasıl hesaplayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Kimliğiyle Göreve Eriş
var task = project.RootTask.Children.GetById(1);

// Takvime ve başlangıç ile bitiş tarihlerine eriş
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Kaynağa ve takvimine eriş
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Dakika Cinsinden Süreyi Al
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// Saat Cinsinden Süreyi Al
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// Gün Cinsinden Süreyi Al
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


