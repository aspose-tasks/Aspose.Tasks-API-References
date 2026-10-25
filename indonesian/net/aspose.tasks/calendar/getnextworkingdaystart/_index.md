---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan"
type: docs
weight: 180
url: /id/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tanggal | DateTime | Tanggal untuk mendapatkan awal hari kerja berikutnya. |

### Nilai Kembali

DateTime awal hari kerja berikutnya.

## Contoh

Menunjukkan cara mendapatkan awal hari kerja berikutnya dengan menggunakan kalender.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan awal hari kerja berikutnya (akhir pekan dilewati)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 April 2020 9:00 AM akan dicetak
Console.WriteLine(nextWorkingDayStart);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


