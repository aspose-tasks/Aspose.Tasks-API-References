---
title: "CalendarCollection.Add"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode CalendarCollection. Menambahkan kalender dasar baru ke objek CalendarCollection ini dan mengembalikan kalender yang ditambahkan"
type: docs
weight: 20
url: /id/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Menambahkan kalender dasar baru ke objek CalendarCollection ini dan mengembalikan kalender yang ditambahkan.

```csharp
public Calendar Add(string name)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | String | Nama kalender. |

### Nilai Kembali

Menambahkan objek [`Calendar`](../../calendar/).

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Dilempar ketika nama kalender bernilai null. |

## Contoh

Menampilkan cara membuat kalender standar.

```csharp
var project = new Project();

// Definisikan kalender dan jadikan standar
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Menambahkan kalender baru dengan kalender dasar yang ditentukan ke objek CalendarCollection ini dan mengembalikan kalender yang ditambahkan.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | String | Nama yang ditentukan. |
| baseCalendar | Calendar | Kalender dasar yang ditentukan. |

### Nilai Kembali

Menambahkan objek [`Calendar`](../../calendar/).

## Contoh

Menampilkan cara menambahkan kalender baru.

```csharp
var project = new Project();

// Kalender baru dapat ditambahkan ke koleksi kalender proyek dengan menggunakan overload Add pada koleksi.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


