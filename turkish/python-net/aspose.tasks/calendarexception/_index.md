---
title: "CalendarException"
second_title: "Aspose.Tasks for Python via .NET API Referansı"
description: 
type: docs
weight: 160
url: /tr/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

Takvimdeki istisnai zaman dilimlerini temsil eder.

CalendarException türü aşağıdaki üyeleri gösterir:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| CalendarException() | Yeni bir [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/) sınıfı örneği başlatır. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| entered_by_occurrences | Tekrarlama aralığının bir sayı girilerek tanımlanıp tanımlanmadığını gösteren bir değeri alır veya ayarlar.<br/>            False, tekrarlama aralığının bir bitiş tarihi girilerek tanımlandığını belirtir. |
| from_date | İstisna zamanının başlangıcını alır veya ayarlar. |
| to_date | İstisna zamanının sonunu alır veya ayarlar. |
| occurrences | Takvim istisnasının geçerli olduğu tekrar sayısını alır veya ayarlar. |
| name | İstisnanın adını alır veya ayarlar. |
| tür | İstisna tipini alır veya ayarlar. |
| period | İstisna için tekrarlama periyodunu alır veya ayarlar. |
| days_of_week | Bu nesne için DayTypeCollection'ı alır.<br/>            İstisnanın geçerli olduğu haftanın günleri. |
| month_item | İstisna tekrarı planlanan ay öğesini alır veya ayarlar. |
| month_position | Bir ay içinde ay öğesinin konumunu alır veya ayarlar. |
| ay | İstisna tekrarı planlanan ayı alır veya ayarlar. |
| month_day | İstisna tekrarı planlanan ayın gününü alır veya ayarlar. |
| day_working | Belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değeri alır veya ayarlar. |
| working_times | WorkingTimeCollection nesnesini alır veya ayarlar.<br/>            Hafta içi çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu. |
| parent_calendar | Bu nesne için üst takvimi alır. |
## Methods
| Ad | Açıklama |
| :- | :- |
| delete() | Exception örneğini üst takvim CalendarExceptionCollection nesnesinden siler. |
| check_exception(dt) | Belirtilen datetime yapısının örneği istisna günü ise true döndürür. |
| get_working_time() | Takvim istisnası için çalışma süresini döndürür. |
| get_exception_dates() | Takvim istisnasının geçerli olduğu tarihleri döndürür. |

### Ayrıca Bakınız

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

