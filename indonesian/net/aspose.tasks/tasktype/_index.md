---
title: "Enum TaskType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.TaskType. Menentukan jenis tugas."
type: docs
weight: 2470
url: /id/net/aspose.tasks/tasktype/
---
## TaskType enumeration

Menentukan jenis tugas.

```csharp
public enum TaskType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Nilai tidak terdefinisi berarti bahwa bidang tersebut tidak didefinisikan dalam file asli |
| FixedUnits | `0` | Unit tetap |
| FixedDuration | `1` | Durasi tetap |
| FixedWork | `2` | Pekerjaan tetap |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara membaca properti default proyek.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Atur properti default
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Tampilkan properti default
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


