---
title: "CalendarCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarCollection yöntemi. Bu koleksiyon için bir enumerator döndürür"
type: docs
weight: 50
url: /tr/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Bu koleksiyon için bir enumerator döndürür.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Dönüş Değeri

bu koleksiyon için bir yineleyici.

## Örnekler

Yeni takvimlerin nasıl ekleneceğini gösterir.

```csharp
var project = new Project();

// Yeni takvimler, bir projenin takvim koleksiyonuna koleksiyonun Add aşırı yüklemeleri kullanılarak eklenebilir.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


