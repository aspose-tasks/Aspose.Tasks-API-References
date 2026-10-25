---
title: "DayTypeCollection.Item"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "DayTypeCollection özelliği. Belirtilen indeksteki öğeyi döndürür veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/daytypecollection/item/
---
## DayTypeCollection indexer

Belirtilen indeksteki öğeyi döndürür veya ayarlar.

```csharp
public DayType this[int index] { get; set; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Alınacak veya ayarlanacak öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

belirtilen indeksteki öğe.

## Örnekler

Haftalık takvim istisnası tanımlamak için bir hafta günü koleksiyonunun nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // "Exception 2" içinden gün tipini gün tipine göre sil
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// "Exception 2" içinden gün tipini indeksine göre sil
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// İstisnaları değiştir (ilk proje verilerinde istisna yok)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// "Exception 3" için haftanın tüm günlerini kaldır
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### Ayrıca Bakınız

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


