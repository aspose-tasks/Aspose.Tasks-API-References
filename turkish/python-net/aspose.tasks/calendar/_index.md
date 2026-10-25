---
title: "Calendar"
second_title: "Aspose.Tasks for Python via .NET API Referansı"
description: 
type: docs
weight: 140
url: /tr/python-net/aspose.tasks/calendar/
---

## Calendar class

Bir projede kullanılan takvimi temsil eder.

Calendar türü aşağıdaki üyeleri gösterir:
## Özellikler
| Ad | Açıklama |
| :- | :- |
| name | Takvim adını alır veya ayarlar. |
| uid | Takvimin benzersiz tanımlayıcısını alır veya ayarlar. |
| week_days | Bu takvim için WeekDaysCollection'ı alır.<br/>            Takvimi tanımlayan hafta içi günlerinin koleksiyonu. |
| exceptions | CalendarExceptionCollection nesnesini alır.<br/>            Takvimle ilişkili istisnaların koleksiyonu. |
| work_weeks | WorkWeekCollections nesnesini alır.<br/>            Takvimle ilişkili çalışma haftalarının koleksiyonu. |
| is_base_calendar | Takvimin temel bir takvim olup olmadığını gösteren değeri alır. |
| base_calendar | Bu takvimin bağlı olduğu temel takvimi alır veya ayarlar.<br/>            Yalnızca takvim temel bir takvim değilse uygulanabilir. |
| is_baseline_calendar | Takvimin temel çizgi takvimi olup olmadığını gösteren değeri alır veya ayarlar. |
| guid | Takvimin Guid'ini alır. |
| primavera_properties | Primavera formatlarından okunan bir takvim için Primavera'ye özgü özellikler içeren bir nesneyi alır. |
## Methods
| Ad | Açıklama |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Belirtilen bitiş tarihi ve süreye göre başlangıç tarihini döndürür. |
| get_start_date_from_finish_and_duration(finish, duration) | Belirtilen bitiş tarihi ve süreye göre başlangıç tarihini döndürür. |
| get_working_hours(start, finish) | WorkUnit'i döndürür - Belirtilen tarih zaman aralığı için çalışma saatlerinin Başlangıç, Bitiş ve Süresi. |
| get_working_hours(dt) | WorkUnit'i döndürür - Belirtilen tarih zaman aralığı için çalışma saatlerinin Başlangıç, Bitiş ve Süresi. |
| get_finish_date_by_start_and_work(start, work) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| get_finish_date_by_start_and_work(start, work) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| get_intersection_calendar(calendar1, calendar2) | 2 takvimin çalışma programlarının kesişimi üzerinde hesaplamalar yapmak için kullanılabilecek [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) örneğini alır. |
| make_standard_calendar(calendar) | Varsayılan standart takvimi oluşturur. |
| make_24_hour_calendar(calendar) | Verilen takvimi 24 Saatlik Takvim yapar.<br/>            24 Saatlik Takvim, haftanın her gününün 24 saat kesintisiz çalıştığı bir takvimdir. |
| make_night_shift_calendar(calendar) | Verilen takvimi Gece Vardiyası Takvimi olarak ayarlar. |
| delete() | Takvimi projeden kaldırır. |
| is_day_working(dt) | Takvime göre belirtilen günün çalışma günü olup olmadığını belirler. |
| get_working_hours_time_span(start, finish) | Belirtilen tarih aralığındaki çalışma saatlerinin miktarını döndürür. |
| get_task_finish_date_from_duration(task, duration) | Görevin başlangıç tarihinden, bölünmüş parçalarından ve çalışma süresinden görevin bitiş tarih ve saatini hesaplar. |
| get_working_times(dt) | Belirtilen tarih için çalışma zamanlarının [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) koleksiyonunu döndürür. |
| get_previous_working_day_end(date) | Belirtilen tarihten önceki çalışma gününün sonunu hesaplar. |
| get_next_working_day_start(date) | Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar. |
| get_work_start(date) | Belirtilen tarih ve saatten başlayarak bir sonraki çalışma zamanının başlangıcını hesaplar. |
| is_empty() | Takvimin tanımlı çalışma saatleri olup olmadığını döndürür. |

### Ayrıca Bakınız

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

