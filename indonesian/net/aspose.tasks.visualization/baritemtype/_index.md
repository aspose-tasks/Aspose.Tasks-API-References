---
title: "Enum BarItemType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.BarItemType. Tipe item untuk mengubah gaya bar."
type: docs
weight: 2940
url: /id/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Jenis item untuk mengubah gaya bar.

```csharp
public enum BarItemType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Task | `0` | Menunjukkan tipe item bar Tugas. |
| Summary | `1` | Menunjukkan tipe item bar Ringkasan. |
| ProjectSummary | `2` | Menunjukkan tipe item bar Ringkasan Proyek. |
| ManualTask | `3` | Menunjukkan tipe item bar Tugas Manual. |
| InactiveTask | `4` | Menunjukkan tipe item bar Tugas Tidak Aktif. |
| CriticalTask | `5` | Menunjukkan tipe item bar Tugas Kritis. |
| Milestone | `6` | Menunjukkan tipe item bar Tugas Milestone. |
| ManualSummary | `7` | Menunjukkan tipe item bar Ringkasan Manual. |
| Split | `8` | Menunjukkan tipe item bar Terpisah. |
| ExternalTasks | `9` | Menunjukkan tipe item bar Tugas Eksternal. |
| ExternalMilestone | `10` | Menunjukkan tipe item bar tonggak eksternal. |
| Deadline | `11` | Menunjukkan tipe item bar tenggat waktu. |
| Progress | `12` | Menunjukkan tipe item bar kemajuan. |
| StartOnly | `13` | Menunjukkan tipe item bar hanya-mulai. |
| FinishOnly | `14` | Menunjukkan tipe item bar hanya-selesai. |
| DurationOnly | `15` | Menunjukkan tipe item bar hanya-durasi. |
| InactiveMilestone | `16` | Menunjukkan tipe item bar tonggak tidak aktif. |
| InactiveSummary | `17` | Menunjukkan tipe item bar ringkasan tidak aktif. |
| SummaryRollup | `18` | Tipe item bar ringkasan rollup. |

## Contoh

Menampilkan cara menyesuaikan batang tugas dengan menggunakan &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s.

```csharp
var project = new Project();

var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

var task3 = project.RootTask.Children.Add("Task 3");
var rsc1 = project.Resources.Add("Resource 1");
var rsc2 = project.Resources.Add("Resource 2");
var rsc3 = project.Resources.Add("Resource 3");

project.ResourceAssignments.Add(task1, rsc1);
project.ResourceAssignments.Add(task2, rsc2);
project.ResourceAssignments.Add(task3, rsc3);

SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.ThirdsOfMonths
};

var style = new BarStyle
                {
                    ItemType = BarItemType.CriticalTask,
                    LeftBarTextConverter = delegate(Task t)
                    {
                        return string.Format("This task (ID = {0}) is on critical path", t.Get(Tsk.Id));
                    }
                };

var style2 = new BarStyle { BarColor = Color.DarkOrchid, ItemType = BarItemType.Task };

options.BarStyles = new List<BarStyle> { style, style2 };

project.Save(OutDir + "CustomizeTextWithTaskBars_out.pdf", options);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


