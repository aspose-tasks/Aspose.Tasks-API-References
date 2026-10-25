---
title: "Enum GroupOn"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.GroupOn. Menentukan tipe pengelompokan"
type: docs
weight: 810
url: /id/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Menentukan tipe pengelompokan.

```csharp
public enum GroupOn
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| DateDay | `13` | Kelompokkan berdasarkan tanggal per hari. |
| DateEachValue | `10` | Kelompokkan berdasarkan tanggal untuk setiap nilai. |
| DateHour | `12` | Kelompokkan tanggal berdasarkan jam. |
| DateMinute | `11` | Kelompokkan tanggal berdasarkan menit. |
| DateMonth | `16` | Kelompokkan tanggal berdasarkan bulan. |
| DateQtr | `17` | Kelompokkan tanggal berdasarkan kuartal. |
| DateThirdOfMonth | `15` | Kelompokkan tanggal berdasarkan setiap sepertiga bulan. |
| DateWeek | `14` | Kelompokkan tanggal berdasarkan minggu. |
| DateYear | `18` | Kelompokkan tanggal berdasarkan tahun. |
| DurationDays | `23` | Kelompokkan durasi berdasarkan hari. |
| DurationEachValue | `20` | Kelompokkan durasi untuk setiap nilai. |
| DurationHours | `22` | Kelompokkan durasi berdasarkan jam. |
| DurationMinutes | `21` | Kelompokkan durasi berdasarkan menit. |
| DurationMonths | `25` | Kelompokkan durasi berdasarkan bulan. |
| DurationWeeks | `24` | Kelompokkan durasi berdasarkan minggu. |
| EachValue | `0` | Kelompokkan berdasarkan setiap nilai. |
| Interval | `1` | Kelompokkan berdasarkan interval. |
| OutlineEachValue | `30` | Kelompokkan setiap nilai outline. |
| OutlineLevel | `31` | Kelompokkan pada level outline. |
| Pct110 | `45` | Kelompokkan berdasarkan kenaikan penyelesaian 10 persen. |
| Pct125 | `44` | Kelompokkan berdasarkan kenaikan penyelesaian 25 persen. |
| Pct150 | `43` | Kelompokkan berdasarkan kenaikan penyelesaian 50 persen. |
| Pct199 | `42` | Kelompokkan berdasarkan penyelesaian 99 persen. |
| PctEachValue | `40` | Kelompokkan persentase setiap nilai. |
| PctInterval | `41` | Kelompokkan persentase interval. |
| TextEachValue | `50` | Kelompokkan setiap nilai teks. |
| TextPrefix | `51` | Kelompokkan awalan teks. |

## Contoh

Menampilkan cara membaca properti kriteria grup.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// baca pola latar belakang kriteria
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


