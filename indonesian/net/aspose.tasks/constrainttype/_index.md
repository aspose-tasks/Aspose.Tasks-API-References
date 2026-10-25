---
title: "Enum ConstraintType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.ConstraintType. Menentukan batas pada tanggal mulai atau selesai suatu tugas"
type: docs
weight: 330
url: /id/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Menentukan batasan pada tanggal mulai atau selesai tugas.

```csharp
public enum ConstraintType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Nilai tidak didefinisikan dalam file proyek asli. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) dan tanggal [`Finish`](../tsk/finish/) dari [`Task`](../task/) dijadwalkan secepat mungkin dengan memperhatikan tanggal [`Start`](../tsk/start/) dan [`Finish`](../tsk/finish/) induk serta mempertimbangkan [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | `[`Start`](../tsk/start/) dan tanggal [`Finish`](../tsk/finish/) dari [`Task`](../task/) dijadwalkan ALAP relatif terhadap [`Start`](../tsk/start/) dan [`Finish`](../tsk/finish/) induk serta mempertimbangkan [`TaskLinks`](../project/tasklinks/).` |
| MustStartOn | `2` | Harus Mulai Pada |
| MustFinishOn | `3` | Harus Selesai Pada |
| StartNoEarlierThan | `4` | Mulai Tidak Lebih Awal Dari |
| StartNoLaterThan | `5` | Mulai Tidak Lebih Lambat Dari |
| FinishNoEarlierThan | `6` | Selesai Tidak Lebih Awal Dari |
| FinishNoLaterThan | `7` | Selesai Tidak Lebih Lambat Dari |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara mengatur batasan &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible untuk sebuah tugas.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Atur batasan As Soon As Possible untuk tugas dengan Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


