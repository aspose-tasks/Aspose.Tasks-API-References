---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ICalendar. Menghitung tanggal dan waktu selesai tugas dari bagian-bagian tanggal mulai dan durasi kerja."
type: docs
weight: 50
url: /id/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Menghitung tanggal dan waktu selesai tugas dari tanggal mulainya, bagian-bagian terpisah, dan durasi kerja.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tugas | Tugas | Tugas untuk menghitung tanggal selesai. |
| durasi | TimeSpan | Durasi yang akan dihitung. |

### Nilai Kembali

Tanggal selesai tugas untuk tanggal mulai dan durasi yang diberikan.

## Catatan

Mengembalikan DateTime.MinValue jika tugas adalah ringkasan, null, atau tanggal mulainya tidak diatur.

### Lihat Juga

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


