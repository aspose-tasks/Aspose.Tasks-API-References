---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Takvime göre belirtilen çalışma süresi geçtiğinde tarihi hesaplar."
type: docs
weight: 160
url: /tr/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Başlangıç tarihi. |
| çalışma | Süre | Çalışma süresi. |

### Dönüş Değeri

Bitiş tarihi.

## Örnekler

Bir takvim örneği kullanarak başlangıç tarihi ve çalışma süresine göre bitiş tarihinin nasıl hesaplanacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// standart bir takvim kullanarak bitiş tarihini hesapla
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Ayrıca Bakınız

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Başlangıç tarihi. |
| çalışma | TimeSpan | Çalışma süresi. |

### Dönüş Değeri

Bitiş tarihi.

## Örnekler

Bir takvim örneği kullanarak başlangıç tarihi ve çalışma süresi (zaman aralığı olarak) ile bitiş tarihinin nasıl hesaplanacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// standart bir takvim kullanarak bitiş tarihini hesapla
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


