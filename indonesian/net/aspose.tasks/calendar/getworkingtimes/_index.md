---
title: "Calendar.GetWorkingTimes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Mengembalikan WorkingTimeCollection dari waktu kerja untuk tanggal yang ditentukan"
type: docs
weight: 240
url: /id/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Mengembalikan [`WorkingTimeCollection`](../../workingtimecollection/) dari waktu kerja untuk tanggal yang ditentukan.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | DateTime | Tanggal untuk mendapatkan waktu kerja. |

### Nilai Kembali

Koleksi instance [`WorkingTime`](../../workingtime/).

## Contoh

Menampilkan cara mendapatkan waktu kerja untuk tanggal tertentu.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan waktu kerja untuk tanggal tertentu
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16 jam akan dicetak
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### Lihat Juga

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


