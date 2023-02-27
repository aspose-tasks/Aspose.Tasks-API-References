---
title: Class Calendar
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.Calendar sınıf. Bir projede kullanılan bir takvimi temsil eder.
type: docs
weight: 230
url: /tr/net/aspose.tasks/calendar/
---
## Calendar class

Bir projede kullanılan bir takvimi temsil eder.

```csharp
public class Calendar
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Bu takvimin bağlı olduğu temel takvimi alır veya ayarlar. Yalnızca takvim bir temel takvim değilse uygulanabilir. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | CalendarExceptionCollection nesnesini alır. Calendar. ile ilişkili istisnalar koleksiyonunu alır. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Takvimin temel takvim olup olmadığını gösteren bir değer alır. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Takvimin temel bir takvim olup olmadığını gösteren bir değer alır veya ayarlar. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Takvimin adını alır veya ayarlar. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Takvimin benzersiz tanımlayıcısını alır veya ayarlar. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Bu takvim için WeekDaysCollection'ı alır. Takvimi tanımlayan hafta içi günleri koleksiyonu. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | WorkWeekCollections nesnesini alır. Takvimle ilişkili çalışma haftaları koleksiyonu. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Belirli bir Takvimi 24 Saatlik Takvim yapar. 24 Saatlik Takvim, haftanın her gününün 24 saat çalışma saatleri ile çalıştığı bir Takvimdir. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Belirli bir Takvimi Gece Vardiyası Takvimi yapar. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Varsayılan standart takvimi oluşturur. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Takvimi projeden kaldırır. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Takvime göre belirtilen çalışma süresinin geçeceği tarihi hesaplar. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Takvime göre belirtilen çalışma süresinin geçeceği tarihi hesaplar. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Sınıfın örneği için bir karma kod döndürür. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Bir sonraki iş günü başlangıç tarihinden itibaren hesaplar. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Belirtilen tarihten önceki çalışma tarihi bitişini hesaplar. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Belirtilen BitişTarihi ve Süreye göre BaşlangıçTarihi'ni döndürür. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Belirtilen BitişTarihi ve Süreye göre BaşlangıçTarihi'ni döndürür. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Görev bitiş tarihini ve saatini başlangıç tarihinden, bölünmüş kısımlardan ve süreden hesaplar. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Tarihteki çalışma saatlerinin miktarını döndürür. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Belirtilen tarihler için çalışma saatlerini iade edin. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | İade[`WorkingTimeCollection`](../workingtimecollection/) belirtilen tarih için çalışma saatleri. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Günün iş günü olup olmadığını belirler. |

### Notlar

Takvimler, standart çalışma ve çalışma dışı saatleri tanımlamak için kullanılır. Projelerin bir temel takvimi olmalıdır. Görevler ve kaynaklar, bir temel takvime dayalı kendi temel olmayan takvimlerine sahip olabilir.

### Örnekler

Sıfırdan basit bir takvim nasıl oluşturulur.

```csharp
[C#]
// boş takvim oluştur
Calendar calendar = new Calendar("New calendar");
// varsayılan çalışma günlerini ekler (9:00 - 17:00 arası 8 çalışma saati)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// yeni yeni iş günü oluştur
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Çalışma süresini ayarlar. DateTime'ın yalnızca zaman kısmı önemlidir
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// hafta sonu ekler
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' boş takvim oluştur
Dim calendar As Calendar =  New Calendar("New calendar")
' varsayılan çalışma günlerini ekler (9:00 - 17:00 arası 8 çalışma saati)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' yeni yeni iş günü oluştur
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Çalışma süresini ayarlar. DateTime'ın yalnızca zaman kısmı önemlidir
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' hafta sonu ekler
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


