---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan"
type: docs
weight: 200
url: /id/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| selesai | DateTime | Tanggal selesai yang ditentukan. |
| durasi | Durasi | Durasi yang ditentukan. |

### Nilai Kembali

Tanggal mulai yang dihitung.

## Contoh

Menampilkan cara mendapatkan tanggal mulai berdasarkan tanggal selesai dan durasi.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan tanggal mulai berdasarkan tanggal selesai dan durasi
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 April 2020 9:00 AM akan dicetak
Console.WriteLine(startDate);
```

### Lihat Juga

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| selesai | DateTime | Tanggal selesai yang ditentukan. |
| durasi | TimeSpan | Durasi yang ditentukan. |

### Nilai Kembali

Tanggal mulai yang dihitung.

## Contoh

Menampilkan cara mendapatkan tanggal mulai berdasarkan tanggal selesai dan durasi (sebagai rentang waktu).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan tanggal mulai berdasarkan tanggal selesai dan durasi
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 April 2020 9:00 AM akan dicetak
Console.WriteLine(startDate);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


