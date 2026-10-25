---
title: "Project.DefaultWeekWorkingDays"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Proje varsayılan hafta çalışma günleri ve çalışma zamanlarını temsil eden WeekDayCollection sınıfının örneğini alır."
type: docs
weight: 370
url: /tr/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Proje varsayılan hafta çalışma günleri ve çalışma zamanlarını temsil eden [`WeekDayCollection`](../../weekdaycollection/) sınıfının örneğini alır.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Dönüş Değeri

Sınıfın [`WeekDayCollection`](../../weekdaycollection/) örneği, [`WeekDay`](../../weekday/) nesnelerinin bir listesini içerir.

## Açıklamalar

Veri yalnızca mpp dosyalarında bulunur (xml içinde değil).

## Örnekler

Varsayılan hafta çalışma gününü nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### Ayrıca Bakınız

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


