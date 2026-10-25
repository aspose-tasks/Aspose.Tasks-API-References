---
title: "Sınıf CalendarCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CalendarCollection sınıfı. Calendar nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 240
url: /tr/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

[`Calendar`](../calendar/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class CalendarCollection : IList<Calendar>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Bu `CalendarCollection` nesnesinde bulunan nesne sayısını döndürür. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Bu CalendarCollection nesnesine yeni bir temel takvim ekler ve eklenen takvimi döndürür. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Bu CalendarCollection nesnesine belirtilen temel takvimle yeni bir takvim ekler ve eklenen takvimi döndürür. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Belirtilen ada sahip bir takvimi döndürür. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Belirtilen UID'ye sahip bir takvimi döndürür. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Takvimi Proje CalendarCollection'dan kaldırır. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | CalendarCollection nesnesini [`Calendar`](../calendar/) nesnelerinin bir listesine dönüştürür. |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


