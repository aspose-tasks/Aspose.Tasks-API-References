---
title: "DayTypeCollection.Item"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "DayTypeCollection property. Mengembalikan atau mengatur elemen pada indeks yang ditentukan"
type: docs
weight: 30
url: /id/net/aspose.tasks/daytypecollection/item/
---
## DayTypeCollection indexer

Mengembalikan atau mengatur elemen pada indeks yang ditentukan.

```csharp
public DayType this[int index] { get; set; }
```

| Parameter | Deskripsi |
| --- | --- |
| index | Indeks berbasis nol dari elemen yang akan diambil atau diatur. |

### Nilai Kembali

elemen pada indeks yang ditentukan.

## Contoh

Menampilkan cara menggunakan koleksi hari minggu untuk mendefinisikan pengecualian kalender mingguan.

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
    // hapus tipe hari dari \"Exception 2\" berdasarkan tipe hari
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// hapus tipe hari dari \"Exception 2\" berdasarkan indeks
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Ubah pengecualian (tidak ada pengecualian dalam data proyek awal)
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

// hapus semua hari minggu untuk \"Exception 3\"
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

### Lihat Juga

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


