---
title: "Enum DateLabel"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.DateLabel. Menentukan format tampilan untuk label tanggal dan waktu dalam skala waktu"
type: docs
weight: 2980
url: /id/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Menentukan format tampilan untuk label tanggal dan waktu dalam skala waktu.

```csharp
public enum DateLabel
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `35` | Tidak ada tanggal yang ditampilkan. |
| DayDdd | `19` | Contohnya Mon, Tue. |
| DayDddDd | `105` | Contohnya Mon 30, Tue 1 |
| DayDddMDd | `112` | Contohnya Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | Contohnya Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | Contohnya Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | Contohnya Mon Sep 30, Tue Oct 1 |
| DayDddMmmDdYyy | `22` | Contohnya Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | Contohnya Mon September 30, Tue October 1 |
| DayDddd | `18` | Contohnya Tuesday, Wednesday. |
| DayDdi | `119` | Contohnya Mo, Tu |
| DayDdiDd | `106` | Contohnya Mo 30, Tu 1 |
| DayDdiMDd | `113` | Contohnya Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Contohnya Mo 9/30, Tu 10/1 |
| DayDi | `20` | Contohnya M, T |
| DayDiDdSpace | `107` | Contohnya M 30, T 1 |
| DayDiMDd | `114` | Contohnya M S 30, T O 1 |
| DayDiMmDd | `110` | Contohnya M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Contohnya M30, T1 |
| DayMDd | `115` | Contohnya S 30, O 1 |
| DayMmDd | `27` | Contohnya 9/30, 10/1 |
| DayMmDdYy | `26` | Contohnya 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Contoh adalah Sep 30, Okt 1 |
| DayMmmDdYyy | `24` | Contoh adalah Sep 30 '02, Okt 10 '02 |
| DayFromEndDayDd | `41` | Contoh adalah Hari 2, Hari 1, Hari -1, Hari -2 dari akhir proyek. |
| DayFromEndDd | `54` | Contoh adalah 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Contoh adalah D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Contoh adalah Hari -2, Hari -1, Hari 1, Hari 2 dari awal proyek. |
| DayFromStartDd | `56` | Contoh adalah -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Contoh adalah D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Contoh adalah 30, 1 |
| DayOfYearDd | `118` | Contoh adalah 77, 78 |
| DayOfYearDdYyy | `116` | Contoh adalah 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Contoh adalah 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Contoh adalah 19/07/2016. |
| HalfYearH | `128` | Contoh adalah 1, 2. Memerlukan satuan waktu menjadi TimescaleHalfYears. |
| HalfYearHh | `127` | Contoh adalah H1, H2 |
| HalfYearHhYyy | `126` | Contoh adalah H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Contoh adalah 1st Half, 2d Half |
| HalfYearHHyy | `129` | Contoh adalah 1H10, 2H10 |
| HalfYearHlfH | `125` | Contoh adalah Setengah 1, Setengah 2 |
| HalfYearHlfHYyyy | `124` | Contoh adalah Setengah 1, 2010; Setengah 2, 2010 |
| HalfYearFromEndH | `135` | Contoh adalah 2, 1, -1, -2. Setengah tahun dari tanggal akhir proyek. |
| HalfYearFromEndHalfH | `133` | Contoh adalah Setengah 2, Setengah 1, Setengah -1, Setengah -2 |
| HalfYearFromEndHh | `134` | Contoh adalah H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Contoh adalah -2, -1, 1, 2. Setengah tahun dari tanggal mulai proyek. |
| HalfYearFromStartHalfH | `130` | Contoh adalah Setengah -2, Setengah -1, Setengah 1, Setengah 2 |
| HalfYearFromStartHh | `131` | Contoh adalah H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Contoh adalah Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Memerlukan satuan waktu menjadi TimescaleHours. |
| HourHh | `32` | Contoh adalah 8, 9, 10, 11 |
| HourHhMmAm | `30` | Contoh adalah 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Contoh adalah 8AM, 9AM |
| HourMmDdHhAm | `120` | Contoh adalah 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Contoh adalah Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | Contoh adalah 3, 2, 1, -1, -2 jam dari akhir proyek. |
| HourFromEndHhh | `76` | Contoh adalah H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Contoh adalah Jam 3, Jam 2, Jam 1, Jam -1, Jam -2 |
| HourFromStartHh | `79` | Contoh adalah -2, -1, 1, 2, 3 jam dari awal proyek. |
| HourFromStartHhh | `78` | Contoh adalah H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Contoh adalah Jam -2, Jam -1, Jam 1, Jam 2, Jam 3 |
| MinuteHhMmAm | `33` | Contoh adalah 8:00 AM, 8:01 AM, 8:02 AM. Memerlukan satuan waktu menjadi TimescaleMinutes. |
| MinuteMm | `34` | Contoh adalah 0, 1, 2, ..., 59 menit |
| MinuteFromEndMinuteMm | `37` | Contoh adalah Menit 181, Menit 180, ..., Menit 1, Menit -1 dari akhir proyek. |
| MinuteFromEndMm | `81` | Contoh adalah 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Contoh adalah M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Contoh adalah Menit -2, Menit -1, Menit 1, ... Menit 180 dari awal proyek. |
| MinuteFromStartMm | `83` | Contoh adalah -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Contoh adalah M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Contoh adalah M, A, M, J, J. Memerlukan satuan waktu menjadi TimescaleMonths. |
| MonthMm | `57` | Contoh adalah 11, 12, 1, 2 |
| MonthMmYy | `86` | Contoh adalah 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Contoh adalah 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Contoh adalah Mar, Apr, Mei |
| MonthMmmYyy | `8` | Contoh adalah Mar '10, Apr '10, Mei '10 |
| MonthMmmm | `9` | Contoh adalah Maret, April, Mei |
| MonthMmmmYyyy | `7` | Contoh adalah Maret 2010, April 2010, Mei 2010 |
| MonthFromEndMm | `59` | Contoh adalah 2, 1, -1, -2 bulan dari akhir proyek. |
| MonthFromEndMmm | `58` | Contoh adalah M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Contoh adalah Bulan 2, Bulan 1, Bulan -1, Bulan -2 |
| MonthFromStartMm | `61` | Contoh adalah -2, -2, 1, 2 bulan dari awal proyek. |
| MonthFromStartMmm | `60` | Contoh adalah M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Contoh adalah Bulan -2, Bulan -1, Bulan 1, Bulan 2 |
| QuarterQ | `62` | Contoh adalah 3, 4, 1. Membutuhkan satuan waktu menjadi TimescaleQuarters. |
| QuarterQq | `6` | Contoh adalah Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Contoh adalah Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Contoh adalah Kuartal ke-3, Kuartal ke-1 |
| QuarterQQyy | `51` | Contoh adalah 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Contoh adalah Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Contoh adalah Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Contoh adalah 5, 4, 3, 2, 1, -1 kuartal dari akhir proyek. |
| QuarterFromEndQq | `63` | Contoh adalah Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Contoh adalah Kuartal 5, Kuartal 4, Kuartal 3, Kuartal 2, Kuartal 1, Kuartal -1 |
| QuarterFromStartQ | `66` | Contoh adalah -5, -4, -3, -2, -1, 1 kuartal dari awal proyek. |
| QuarterFromStartQq | `65` | Contoh adalah Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Contoh adalah Kuartal -5, Kuartal -4, Kuartal -3, Kuartal -2, Kuartal -1, Kuartal 1 |
| ThirdsOfMonthsDd | `136` | Contoh adalah 1, 11, 21, 1. Membutuhkan satuan waktu menjadi TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Contoh adalah B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Contoh adalah Awal, Tengah, Akhir, Awal |
| ThirdsOfMonthsMmDd | `139` | Contoh adalah 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Contoh adalah 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Contoh adalah 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Contoh adalah 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Contoh adalah Mar 1, Mar 11, Mar 21, Apr 1 |
| ThirdsOfMonthsMmmDdYy | `147` | Contoh adalah Mar 1, '10; Mar 11, '10; Mar 21, '10; Apr 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Contoh adalah Mar B, Mar M, Mar E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Contoh adalah Mar B, '10; Mar M, '10; Mar E, '10; Apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Contoh adalah Maret 1, Maret 11, Maret 21, April 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Contoh adalah Maret 1, 2010; Maret 11, 2010; Maret 21, 2010; April 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Contoh adalah Maret Awal, Maret Tengah, Maret Akhir, April Awal |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Contoh adalah Maret Awal, 2010; Maret Tengah, 2010; Maret Akhir, 2010; April Awal, 2010 |
| WeekDddDd | `88` | Contoh adalah Ming 21, Ming 28, Ming 4. Membutuhkan satuan waktu menjadi TimescaleWeeks. |
| WeekDddMDd | `97` | Contoh adalah Ming M 21, Ming M 28, Ming A 4 |
| WeekDddMmDd | `90` | Contoh adalah Ming 3/21, Ming 3/28, Ming 4/4 |
| WeekDddMmDdYy | `100` | Contoh adalah Ming 3/21/10, Ming 3/28/10, Ming 4/4/10 |
| WeekDddMmmDd | `93` | Contoh adalah Ming Mar 21, Ming Mar 28, Ming Apr 4 |
| WeekDddMmmDdYyy | `101` | Contoh adalah Ming Mar 21, '10; Ming Mar 28, '10; Ming Apr 4, '10 |
| WeekDddMmmmDd | `96` | Contoh adalah Ming Mar 21, Ming Maret 28, Ming Apr 4 |
| WeekDddMmmmDdYyy | `102` | Contoh adalah Ming Maret 21, '10; Ming Maret 28, '10; Ming April 4, '10 |
| WeekDddWw | `103` | Contoh adalah Ming 12, Ming 13, Ming 14 |
| WeekDdiMDd | `98` | Contoh adalah Ming M 21, Ming M 28, Ming A 4 |
| WeekDdiMmDd | `91` | Contoh adalah Ming 3/21. Ming 3/28, Ming 4/4 |
| WeekDdiMmmDd | `94` | Contoh adalah Ming Mar 21, Ming Mar 28, Ming Apr 4 |
| WeekDiMDd | `99` | Contoh adalah S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Contoh adalah S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Contoh adalah S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | Contoh adalah M21, M28, A 4 |
| WeekMmDd | `17` | Contoh adalah 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Contoh adalah '3/21/10'. |
| WeekMmmDd | `15` | Contoh adalah Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | Contoh adalah Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | Contoh adalah March 21, March 28, April 4 |
| WeekMmmmDdYyyy | `12` | Contoh adalah March 21, 2010; March 28, 2010; April 4, 2010 |
| WeekDayOfMonthDd | `87` | Contoh adalah 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Contoh adalah Week 2, Week 1, Week -1 dari akhir proyek. |
| WeekFromEndWw | `68` | Contoh adalah 2, 1, -1 |
| WeekFromEndWww | `67` | Contoh adalah W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Contoh adalah Week -1, Week 1, Week 2 dari awal proyek. |
| WeekFromStartWw | `70` | Contoh adalah -1, 1, 2 |
| WeekFromStartWww | `69` | Contoh adalah W-1, W1, W2 |
| WeekNumberDdWw | `104` | Contoh adalah 1 12, 1 13, 1 14 (hari 1 minggu ke-12, hari 1 minggu ke-13, dan seterusnya) |
| WeekNumberWw | `50` | Contoh adalah 12, 13, 14 |
| YearYy | `75` | Contoh adalah 10, 11, 12. Membutuhkan satuan waktu menjadi TimescaleYears. |
| YearYyy | `1` | Contoh adalah '10, '11, '12 |
| YearYyyy | `0` | Contoh adalah 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Contoh adalah Year 2, Year 1, Year -1 dari akhir proyek. |
| YearFromEndYy | `72` | Contoh adalah 2, 1, -1 |
| YearFromEndYyy | `71` | Contoh adalah Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Contoh adalah Year -1, Year 1, Year 2 dari awal proyek. |
| YearFromStartYy | `74` | Contoh adalah -1, 1, 2 |
| YearFromStartYyy | `73` | Contoh adalah Y-1, Y1, Y2 |

## Contoh

Menampilkan cara menyesuaikan label tingkat skala waktu.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Tambahkan tautan tugas
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// sesuaikan tingkat skala waktu

// sesuaikan tingkat atas
// atur tingkat skala waktu atas pada tampilan Diagram Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// atur satuan skala waktu <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> untuk tingkat skala waktu.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// atur interval satuan waktu di mana label ditampilkan untuk tingkat.
view.MiddleTimescaleTier.Count = 1;
// atur label tanggal <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> untuk tingkat skala waktu.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// atur cara menyejajarkan label dalam setiap periode waktu tingkat (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// atur nilai yang menunjukkan apakah menampilkan tanda centang yang memisahkan periode waktu dalam tingkat.
view.MiddleTimescaleTier.ShowTicks = true;
// atur nilai yang menunjukkan apakah mendasarkan label tingkat pada tahun fiskal.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// ditambahkan untuk visualisasi yang lebih baik
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// sesuaikan tanggal tingkat tengah
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Gunakan opsi 'Timescale.DefinedInView' untuk merender skala waktu menggunakan pengaturan skala waktu yang didefinisikan dalam tampilan (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


