---
title: "Calendar.GetWorkingHours"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Mengembalikan WorkUnit Start Finish dan Durasi jam kerja untuk interval tanggal-waktu yang ditentukan."
type: docs
weight: 220
url: /id/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Kembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai interval. |
| selesai | DateTime | Tanggal selesai interval. |

### Nilai Kembali

Instance kelas [`WorkUnit`](../../workunit/) yang berisi Start, Finish, dan Duration jam kerja.

## Contoh

Menampilkan cara mendapatkan jam kerja untuk tanggal tertentu.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan jam kerja untuk tanggal tertentu
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16 jam akan dicetak
Console.WriteLine(workUnit.WorkingHours);
```

### Lihat Juga

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Mengembalikan jumlah jam kerja pada tanggal yang ditentukan.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | DateTime | Tanggal untuk mendapatkan jam kerja. |

### Nilai Kembali

Jam kerja pada tanggal yang ditentukan.

## Contoh

Menampilkan cara mendapatkan jam kerja untuk tanggal tertentu.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan jam kerja untuk tanggal tertentu
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 8 jam akan dicetak
Console.WriteLine(workingHours.Hours);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


