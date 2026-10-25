---
title: "Kelas EndAfterRecurrenceRange"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.EndAfterRecurrenceRange. Mewakili rentang pengulangan tugas berulang yang dibatasi oleh jumlah kejadian"
type: docs
weight: 500
url: /id/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

Mewakili rentang pengulangan tugas berulang yang dibatasi oleh jumlah kejadian.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | Menginisialisasi instance baru dari kelas `EndAfterRecurrenceRange`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | Mendapatkan atau mengatur jumlah kejadian yang membatasi rentang pengulangan tugas berulang. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Mendapatkan atau mengatur tanggal mulai rentang pengulangan tugas berulang. |

## Contoh

Menampilkan cara bekerja dengan pengulangan pola kerja harian saat membuat tugas berulang.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// lanjutkan bekerja dengan proyek...
// ...
```

### Lihat Juga

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


