---
title: "Enum TaskStartDateType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.TaskStartDateType enum. Menentukan jenis tanggal mulai tugas"
type: docs
weight: 2450
url: /id/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Menentukan jenis tanggal mulai tugas.

```csharp
public enum TaskStartDateType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Nilai bidang tidak didefinisikan dalam file proyek asli. |
| ProjectStartDate | `0` | Tanggal mulai proyek |
| CurrentDate | `1` | Tanggal saat ini |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara mengatur tanggal mulai default tugas sebagai 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


