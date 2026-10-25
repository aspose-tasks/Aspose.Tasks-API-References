---
title: "Calendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Belirtilen tarih zaman aralığı için çalışma saatlerinin WorkUnit, Başlangıç, Bitiş ve Süresini döndürür."
type: docs
weight: 220
url: /tr/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

WorkUnit'i döndürür - Belirtilen tarih saat aralığı için çalışma saatlerinin Başlangıç, Bitiş ve Süresi.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Aralığın başlangıç tarihi. |
| bitiş | DateTime | Aralığın bitiş tarihi. |

### Dönüş Değeri

[`WorkUnit`](../../workunit/) sınıfının, çalışma saatlerinin Başlangıç, Bitiş ve Süresini içeren örneği.

## Örnekler

Belirli tarihler için çalışma saatlerini almanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// Belirli bir tarih için çalışma saatlerini al.
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16 saat yazdırılacak
Console.WriteLine(workUnit.WorkingHours);
```

### Ayrıca Bakınız

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Belirtilen tarihteki çalışma saatlerinin miktarını döndürür.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | DateTime | Çalışma saatlerini almak için tarih. |

### Dönüş Değeri

Belirtilen tarihteki çalışma saatleri.

## Örnekler

Belirli bir tarih için çalışma saatlerini almanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// Belirli bir tarih için çalışma saatlerini al.
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 8 saat yazdırılacak
Console.WriteLine(workingHours.Hours);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


