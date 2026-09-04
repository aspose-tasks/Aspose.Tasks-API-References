---
title: "Aspose::Tasks::Calendar sınıfı"
linktitle: "Takvim"
articleTitle: "Takvim"
second_title: "C++ için Aspose.Tasks"
description: "Bir projede kullanılan takvimi temsil eder."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Bir projede kullanılan takvimi temsil eder.

Sıfırdan basit bir takvim nasıl oluşturulur.

```cpp
[C#]
// boş takvim oluştur
Calendar calendar = new Calendar("New calendar");
// varsayılan çalışma günlerini ekler (9:00'dan 17:00'ye kadar 8 çalışma saati)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// yeni bir çalışma günü oluştur
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Çalışma zamanını ayarlar. Yalnızca DateTime'in zaman kısmı önemlidir.
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

```cpp
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

Takvimler, standart çalışma ve çalışma dışı zamanları tanımlamak için kullanılır. Projelerin bir temel takvimi olmalıdır. Görevler ve kaynaklar, temel takvime dayalı kendi temel olmayan takvimlerine sahip olabilir.

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Delete](./delete/) | Projeden takvimi kaldırır. |
| [Equals](./equals/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [get_BaseCalendar](./get_basecalendar/) | Bu takvimin bağlı olduğu temel takvimi alır. Takvim bir temel takvim değilse yalnızca uygulanabilir. |
| [get_Exceptions](./get_exceptions/) | CalendarExceptionCollection nesnesini alır. Takvimle ilişkili istisnaların koleksiyonu. |
| [get_Guid](./get_guid/) | Takvimin GUID'ini alır. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Takvimin temel takvim olup olmadığını gösteren bir değeri alır. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Takvimin temel takvim olup olmadığını gösteren bir değer alır. |
| [get_Name](./get_name/) | Takvimin adını alır. |
| [get_Uid](./get_uid/) | Takvimin benzersiz tanımlayıcısını alır. |
| [get_WeekDays](./get_weekdays/) | Bu takvim için WeekDaysCollection'ı alır. Takvimi tanımlayan hafta içi günlerinin koleksiyonu. |
| [get_WorkWeeks](./get_workweeks/) | WorkWeekCollections nesnesini alır. Takvimle ilişkili çalışma haftalarının koleksiyonu. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Belirtilen çalışma süresi miktarının takvime göre geçeceği tarihi hesaplar. |
| [GetHashCode](./gethashcode/) | Sınıf örneği için bir karma kod (hash code) döndürür. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | 2 takvimin çalışma programlarının kesişimi üzerinde hesaplamalar yapmak için kullanılabilecek ICalendar örneğini alır. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Belirtilen tarihten önceki çalışma gününün sonunu hesaplar. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Belirtilen bitiş tarihi ve süreye göre başlangıç tarihini döndürür. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Görevin başlangıç tarihi, bölünmüş parçaları ve çalışma süresinden bitiş tarih ve saatini hesaplar. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Belirtilen tarihteki çalışma saatlerinin miktarını döndürür. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Belirtilen tarihler arasındaki çalışma saatlerinin miktarını döndürür. |
| [GetWorkingTimes](./getworkingtimes/) | Belirtilen tarih için çalışma zamanlarının WorkingTimeCollection'ını döndürür. |
| [GetWorkStart](./getworkstart/) | Belirtilen tarih ve saatten başlayarak bir sonraki çalışma zamanının başlangıcını hesaplar. |
| [IsDayWorking](./isdayworking/) | Belirtilen günün takvime göre bir çalışma günü olup olmadığını belirler. |
| [IsEmpty](./isempty/) | Takvimin tanımlı çalışma saatleri olup olmadığını döndürür. |
| [Make24HourCalendar](./make24hourcalendar/) | Verilen takvimi 24 Saat Takvim yapar. 24 Saat Takvim, haftanın her gününün kesintisiz çalışma saatlerine sahip olduğu bir takvimdir. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Verilen takvimi Gece Vardiyası Takvimi yapar. |
| [MakeStandardCalendar](./makestandardcalendar/) | Varsayılan standart takvimi oluşturur. |
| [set_BaseCalendar](./set_basecalendar/) | Bu takvimin bağlı olduğu temel takvimi ayarlar. Yalnızca takvim bir temel takvim değilse uygulanabilir. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Takvimin temel takvim olup olmadığını gösteren bir değeri ayarlar. |
| [set_Name](./set_name/) | Takvimin adını ayarlar. |
| [set_Uid](./set_uid/) | Takvimin benzersiz tanımlayıcısını ayarlar. |

