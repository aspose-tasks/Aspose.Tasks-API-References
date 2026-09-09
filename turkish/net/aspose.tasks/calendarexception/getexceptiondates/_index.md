---
title: "CalendarException.GetExceptionDates"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException yöntemi. Takvim istisnasının geçerli olduğu tarihleri döndürür."
type: docs
weight: 190
url: /tr/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Takvim istisnasının geçerli olduğu tarihleri döndürür.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Dönüş Değeri

Takvim istisnasının geçerli olduğu istisna tarihlerinin bir koleksiyonunu döndürür.

## Örnekler

Belirli bir takvim istisnasının geçerli olduğu tarihleri nasıl alacağınızı gösterir.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### Ayrıca Bakınız

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


