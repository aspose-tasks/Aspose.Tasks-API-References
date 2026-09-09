---
title: "Sınıf Calendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Calendar sınıfı. Bir projede kullanılan takvimi temsil eder."
type: docs
weight: 230
url: /tr/net/aspose.tasks/calendar/
---
## Calendar class

Bir projede kullanılan takvimi temsil eder.

```csharp
public class Calendar : ICalendar
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Bu takvimin bağlı olduğu temel takvimi alır veya ayarlar. Yalnızca takvim bir temel takvim değilse uygulanabilir. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | CalendarExceptionCollection nesnesini alır. Takvimle ilişkili istisna koleksiyonunu içerir. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Takvimin GUID'sini alır. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Takvimin temel takvim olup olmadığını gösteren bir değeri alır. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Takvimin temel çizgi takvimi olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Takvimin adını alır veya ayarlar. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Primavera formatlarından okunan bir takvim için Primavera'ya özgü özellikleri içeren bir nesneyi alır. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Takvimin benzersiz tanımlayıcısını alır veya ayarlar. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Bu takvim için WeekDaysCollection'ı alır. Takvimi tanımlayan hafta içi günlerinin koleksiyonunu içerir. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | WorkWeekCollections nesnesini alır. Takvimle ilişkili çalışma haftalarının koleksiyonunu içerir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Verilen takvimi 24 Saatlik Takvim yapar. 24 Saatlik Takvim, haftanın her gününün 24 saat çalıştığı bir takvimdir. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Verilen Takvimi Gece Vardiyası Takvimi yapar. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Varsayılan standart takvimi oluşturur. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Takvimi projeden kaldırır. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Sınıf örneği için bir karma kodu döndürür. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Belirtilen tarihten önceki çalışma gününün sonunu hesaplar. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Belirtilen bitiş tarihi ve süreye dayanarak başlangıç tarihini döndürür. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Belirtilen bitiş tarihi ve süreye dayanarak başlangıç tarihini döndürür. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Görevin başlangıç tarihi, bölünmüş parçaları ve çalışma süresinden görev bitiş tarih ve saatini hesaplar. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Belirtilen tarihteki çalışma saatlerinin miktarını döndürür. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | WorkUnit'i döndürür - Belirtilen tarih saat aralığı için çalışma saatlerinin Başlangıç, Bitiş ve Süresi. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Belirtilen tarihler arasındaki çalışma saatlerinin miktarını döndürür. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Belirtilen tarih için çalışma zamanlarının [`WorkingTimeCollection`](../workingtimecollection/) koleksiyonunu döndürür. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Belirtilen tarih ve saatten başlayarak bir sonraki çalışma zamanının başlangıcını hesaplar. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Belirtilen günün takvime göre bir çalışma günü olup olmadığını belirler. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Takvimin tanımlı çalışma saatlerine sahip olup olmadığını döndürür. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | 2 takvimin çalışma programlarının kesişimi üzerinde hesaplamalar yapmak için kullanılabilecek [`ICalendar`](../icalendar/) örneğini alır. |

## Açıklamalar

Takvimler, standart çalışma ve tatil zamanlarını tanımlamak için kullanılır. Projelerin bir temel takvimi olmalıdır. Görevler ve kaynaklar, temel takvime dayalı kendi temel dışı takvimlerine sahip olabilir.

## Örnekler

Sıfırdan basit bir takvim nasıl oluşturulur.

```csharp
[C#]
// boş takvim oluştur
Calendar calendar = new Calendar("New calendar");
// varsayılan çalışma günlerini ekler (9:00'dan 17:00'ye kadar 8 çalışma saati)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// yeni bir çalışma günü oluştur
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Çalışma zamanını ayarlar. Yalnızca DateTime'ın zaman kısmı önemlidir.
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
// hafta sonunu ekler
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
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
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

Yeni bir takvim nasıl tanımlanır, haftanın günleri nasıl eklenir ve günler için çalışma zamanları nasıl belirlenir gösterir.

```csharp
var project = new Project();

// Bir takvim tanımla
var calendar = project.Calendars.Add("Calendar1");

// Pazartesiden perşembeye varsayılan zamanlarla çalışma günleri ekle
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Cuma gününü kısa çalışma günü olarak ayarla
var weekDay = new WeekDay(DayType.Friday);

// Çalışma zamanını ayarlar. Yalnızca DateTime'ın zaman kısmı önemlidir.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// projeyle çalışılıyor...
```

### Ayrıca Bakınız

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


