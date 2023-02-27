---
title: Class WeekDay
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.WeekDay sınıf. Bir takvimde haftanın normal günlerini veya istisna günlerini tanımlayan bir hafta içi günü temsil eder.
type: docs
weight: 3180
url: /tr/net/aspose.tasks/weekday/
---
## WeekDay class

Bir takvimde haftanın normal günlerini veya istisna günlerini tanımlayan bir hafta içi günü temsil eder.

```csharp
public class WeekDay
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Yeni bir örneğini başlatır.`WeekDay` sınıf. |
| [WeekDay](weekday/#constructor_1)(DayType) | Yeni bir örneğini başlatır.`WeekDay` belirtilen gün tipine sahip sınıf. |
| [WeekDay](weekday/#constructor_2)(DayType, IEnumerable&lt;WorkingTime&gt;) | Yeni bir örneğini başlatır.`WeekDay` belirtilen gün türü ve çalışma zaman dilimlerinin listesi ile sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Bir günün türünü alır. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değer alır veya ayarlar. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Bir istisna süresinin başlangıcını alır veya ayarlar. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Bir istisna süresinin sonunu alır veya ayarlar. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Bu WeekDay örneği için WorkingTimeCollection'ı alır. Hafta içi çalışılan zamanı tanımlayan çalışma saatleri koleksiyonu. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Varsayılan çalışma günü oluşturur. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Haftanın gününün derin bir kopyasını döndürür. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Örneği için bir karma kod değeri döndürür`WeekDay` sınıf. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Haftanın bir günü için çalışma süresini verir. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | .Net yayınlarDayOfWeek ile[`DayType`](./daytype/) . |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Belirtilen hafta günü için varsayılan zaman dilimlerini ayarlar. |

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


