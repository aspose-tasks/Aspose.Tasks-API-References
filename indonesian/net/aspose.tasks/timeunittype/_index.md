---
title: "Enum TimeUnitType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.TimeUnitType enum. Menentukan tipe satuan waktu."
type: docs
weight: 2570
url: /id/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Menentukan jenis satuan waktu.

```csharp
public enum TimeUnitType : sbyte
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan nilai Undefined berarti bahwa bidang tidak didefinisikan dalam file proyek asli. |
| Minute | `0` | Menunjukkan tipe satuan waktu Menit. |
| ElapsedMinute | `1` | Menunjukkan tipe satuan waktu menit yang telah berlalu. |
| Hour | `2` | Menunjukkan tipe satuan waktu Jam. |
| ElapsedHour | `3` | Menunjukkan tipe satuan waktu jam yang telah berlalu. |
| Day | `4` | Menunjukkan tipe satuan waktu Hari. |
| ElapsedDay | `5` | Menunjukkan tipe satuan waktu hari yang telah berlalu. |
| Week | `6` | Menunjukkan tipe satuan waktu Minggu. |
| ElapsedWeek | `7` | Menunjukkan tipe satuan waktu minggu yang telah berlalu. |
| Month | `8` | Menunjukkan tipe satuan waktu Bulan. |
| ElapsedMonth | `9` | Menunjukkan tipe satuan waktu bulan yang telah berlalu. |
| Percent | `10` | Menunjukkan tipe satuan waktu Persen. |
| ElapsedPercent | `11` | Menunjukkan tipe satuan waktu persen yang telah berlalu. |
| Null | `12` | Menunjukkan tipe satuan waktu Null. |
| MinuteEstimated | `13` | Menunjukkan tipe satuan waktu menit yang diperkirakan. |
| ElapsedMinuteEstimated | `14` | Menunjukkan tipe satuan waktu menit perkiraan yang telah berlalu. |
| HourEstimated | `15` | Menunjukkan tipe satuan waktu jam yang diperkirakan. |
| ElapsedHourEstimated | `16` | Menunjukkan tipe satuan waktu jam perkiraan yang telah berlalu. |
| DayEstimated | `17` | Menunjukkan tipe satuan waktu hari yang diperkirakan. |
| ElapsedDayEstimated | `18` | Menunjukkan tipe satuan waktu hari perkiraan yang telah berlalu. |
| WeekEstimated | `19` | Menunjukkan tipe satuan waktu minggu yang diperkirakan. |
| ElapsedWeekEstimated | `20` | Menunjukkan tipe satuan waktu minggu perkiraan yang telah berlalu. |
| MonthEstimated | `21` | Menunjukkan tipe satuan waktu bulan yang diperkirakan. |
| ElapsedMonthEstimated | `22` | Menunjukkan tipe satuan waktu bulan perkiraan yang telah berlalu. |
| PercentEstimated | `23` | Menunjukkan tipe satuan waktu persen perkiraan. |
| ElapsedPercentEstimated | `24` | Menunjukkan tipe unit waktu perkiraan persentase yang telah berlalu. |
| Year | `25` | Menunjukkan tipe unit waktu Tahun. |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara mengonversi durasi ke dalam berbagai tipe unit waktu.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Dapatkan tugas untuk menghitung durasinya dalam berbagai format
var task = project.RootTask.Children.GetById(1);

// Dapatkan durasi dalam Menit, Hari, Jam, Minggu, dan Bulan
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


