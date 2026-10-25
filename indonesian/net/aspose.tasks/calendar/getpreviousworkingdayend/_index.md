---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Menghitung akhir hari kerja sebelumnya dari tanggal yang ditentukan"
type: docs
weight: 190
url: /id/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tanggal | DateTime | tanggal untuk menghitung akhir hari kerja sebelumnya. |

### Nilai Kembali

Akhir dari akhir hari kerja sebelumnya.

## Contoh

Menampilkan cara mendapatkan akhir hari kerja sebelumnya dengan menggunakan kalender.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan akhir hari kerja sebelumnya
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 9 April 2020 18:00 PM akan dicetak
Console.WriteLine(previousWorkingDayEnd);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


