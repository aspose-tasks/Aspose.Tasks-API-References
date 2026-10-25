---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Belirtilen bitiş tarihi ve süreye göre başlangıç tarihini döndürür."
type: docs
weight: 200
url: /tr/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Belirtilen bitiş tarihi ve süreye dayanarak başlangıç tarihini döndürür.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bitiş | DateTime | Belirtilen bitiş tarihi. |
| süre | Süre | Belirtilen süre. |

### Dönüş Değeri

Hesaplanan başlangıç tarihi.

## Örnekler

Bitiş tarihi ve süreye göre bir başlangıç tarihinin nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// bitiş tarihi ve bir süreye göre başlangıç tarihini al
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 Nisan 2020 9:00 AM yazdırılacak
Console.WriteLine(startDate);
```

### Ayrıca Bakınız

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Belirtilen bitiş tarihi ve süreye dayanarak başlangıç tarihini döndürür.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bitiş | DateTime | Belirtilen bitiş tarihi. |
| süre | TimeSpan | Belirtilen süre. |

### Dönüş Değeri

Hesaplanan başlangıç tarihi.

## Örnekler

Bitiş tarihi ve süreye (zaman aralığı olarak) göre bir başlangıç tarihinin nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// bitiş tarihi ve bir süreye göre başlangıç tarihini al
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 Nisan 2020 9:00 AM yazdırılacak
Console.WriteLine(startDate);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


