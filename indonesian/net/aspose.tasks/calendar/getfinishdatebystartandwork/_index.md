---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender"
type: docs
weight: 160
url: /id/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai. |
| kerja | Durasi | Durasi kerja. |

### Nilai Kembali

Tanggal selesai.

## Contoh

Menampilkan cara menghitung tanggal selesai berdasarkan tanggal mulai dan kerja menggunakan instance kalender.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// hitung tanggal selesai dengan menggunakan kalender standar
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Lihat Juga

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai. |
| kerja | TimeSpan | Durasi kerja. |

### Nilai Kembali

Tanggal selesai.

## Contoh

Menampilkan cara menghitung tanggal selesai berdasarkan tanggal mulai dan kerja (sebagai rentang waktu) menggunakan instance kalender.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// hitung tanggal selesai dengan menggunakan kalender standar
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


