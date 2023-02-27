---
title: DateLabel
second_title: Aspose.Tasks untuk Referensi .NET API
description: Menentukan format tampilan untuk label tanggal dan waktu dalam skala waktu.
type: docs
weight: 2650
url: /id/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Menentukan format tampilan untuk label tanggal dan waktu dalam skala waktu.

```csharp
public enum DateLabel
```

### Nilai

| Nama | Nilai | Keterangan |
| --- | --- | --- |
| None | `35` | Tidak ada tanggal yang ditampilkan. |
| DayDdd | `19` | Contohnya adalah Sen, Sel. |
| DayDddDd | `105` | Contohnya Sen 30, Sel 1 |
| DayDddMDd | `112` | Contohnya adalah Sen S 30, Sel O 1 |
| DayDddMmDd | `108` | Contohnya Senin 30/9, Selasa 10/1_x000h_ |
| DayDddMmDdYy | `52` | Contohnya adalah Senin 30/9/02, Sel 1/10/02 |
| DayDddMmmDd | `23` | Contohnya adalah Sen 30 Sep, Sel 1 Okt |
| DayDddMmmDdYyy | `22` | Contohnya adalah Sen 30 Sep '02, Sel 1 Okt '02 |
| DayDddMmmmDd | `111` | Contohnya Senin 30 September, Selasa 1 Oktober |
| DayDddd | `18` | Contohnya Selasa, Rabu. |
| DayDdi | `119` | Contohnya adalah Mo, Tu |
| DayDdiDd | `106` | Contohnya Mo 30, Tu 1 |
| DayDdiMDd | `113` | Contohnya adalah Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Contohnya Mo 9/30, Tu 10/1 |
| DayDi | `20` | Contohnya adalah M, T |
| DayDiDdSpace | `107` | Contohnya adalah M 30, T 1 |
| DayDiMDd | `114` | Contohnya MS 30, TO 1 |
| DayDiMmDd | `110` | Contohnya adalah M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Contohnya adalah M30, T1 |
| DayMDd | `115` | Contohnya adalah S 30, O 1 |
| DayMmDd | `27` | Contohnya adalah 9/30, 10/1 |
| DayMmDdYy | `26` | Contohnya adalah 30/9/02, 1/10/02 |
| DayMmmDd | `25` | Contohnya adalah 30 Sep, 1 Okt |
| DayMmmDdYyy | `24` | Contohnya adalah Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | Contohnya adalah Hari 2, Hari 1, Hari -1, Hari -2 dari akhir proyek. |
| DayFromEndDd | `54` | Contohnya adalah 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Contohnya adalah D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Contohnya adalah Hari -2, Hari -1, Hari 1, Hari 2 sejak proyek dimulai. |
| DayFromStartDd | `56` | Contohnya adalah -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Contohnya D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Contohnya adalah 30, 1 |
| DayOfYearDd | `118` | Contohnya adalah 77, 78 |
| DayOfYearDdYyy | `116` | Contohnya adalah 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Contohnya adalah 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Contoh 19/07/2016. |
| HalfYearH | `128` | Contohnya adalah 1, 2. Membutuhkan satuan waktu TimescaleHalfYears. |
| HalfYearHh | `127` | Contohnya adalah H1, H2 |
| HalfYearHhYyy | `126` | Contohnya adalah H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Contohnya adalah Babak ke-1, Babak ke-2 |
| HalfYearHHyy | `129` | Contohnya adalah 1H10, 2H10 |
| HalfYearHlfH | `125` | Contohnya adalah Separuh 1, Separuh 2 |
| HalfYearHlfHYyyy | `124` | Contohnya adalah Setengah 1, 2010; Setengah 2, 2010 |
| HalfYearFromEndH | `135` | Contohnya adalah 2, 1, -1, -2. Setengah tahun dari tanggal akhir proyek. |
| HalfYearFromEndHalfH | `133` | Contohnya adalah Separuh 2, Separuh 1, Separuh -1, Separuh -2 |
| HalfYearFromEndHh | `134` | Contohnya adalah H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Contohnya adalah -2, -1, 1, 2. Setengah tahun dari tanggal mulai proyek. |
| HalfYearFromStartHalfH | `130` | Contohnya adalah Separuh -2, Separuh -1, Separuh 1, Separuh 2 |
| HalfYearFromStartHh | `131` | Contohnya adalah H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Contohnya adalah Rab 18 Mar, 8 AM; Rab 18 Mar, 09:00. Membutuhkan satuan waktu menjadi TimescaleHours. |
| HourHh | `32` | Contohnya adalah 8, 9, 10, 11 |
| HourHhMmAm | `30` | Contohnya adalah 08.00, 09.00 |
| HourHhAm | `31` | Contohnya adalah 8AM, 9AM |
| HourMmDdHhAm | `120` | Contohnya adalah 18/3 8 pagi, 18/3 9 pagi |
| HourMmmDdHhAm | `29` | Contohnya adalah 18 Maret, 8 pagi; 18 Mar 09.00 |
| HourFromEndHh | `77` | Contohnya adalah 3, 2, 1, -1, -2 jam dari proyek berakhir. |
| HourFromEndHhh | `76` | Contohnya adalah H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Contohnya adalah Jam 3, Jam 2, Jam 1, Jam -1, Jam -2 |
| HourFromStartHh | `79` | Contohnya adalah -2, -1, 1, 2, 3 jam sejak proyek dimulai. |
| HourFromStartHhh | `78` | Contohnya adalah H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Contohnya adalah Jam -2, Jam -1, Jam 1, Jam 2, Jam 3 |
| MinuteHhMmAm | `33` | Contohnya adalah 08.00, 08.01, 08.02. Membutuhkan satuan waktu menjadi TimescaleMinutes. |
| MinuteMm | `34` | Contohnya adalah 0, 1, 2, ..., 59 menit |
| MinuteFromEndMinuteMm | `37` | Contohnya adalah Menit 181, Menit 180, ..., Menit 1, Menit -1 dari akhir proyek. |
| MinuteFromEndMm | `81` | Contohnya adalah 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Contohnya adalah M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Contohnya adalah Menit -2, Menit -1, Menit 1, ... Menit 180 dari awal proyek. |
| MinuteFromStartMm | `83` | Contohnya adalah -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Contohnya adalah M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Contohnya adalah M, A, M, J, J. Membutuhkan satuan waktu menjadi TimescaleMonths. |
| MonthMm | `57` | Contohnya adalah 11, 12, 1, 2 |
| MonthMmYy | `86` | Contohnya adalah 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Contohnya adalah 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Contohnya adalah Mar, Apr, May |
| MonthMmmYyy | `8` | Contohnya Mar '10, Apr '10, Mei '10 |
| MonthMmmm | `9` | Contohnya Maret, April, Mei |
| MonthMmmmYyyy | `7` | Contohnya Maret 2010, April 2010, Mei 2010 |
| MonthFromEndMm | `59` | Contohnya adalah 2, 1, -1, -2 bulan dari akhir proyek. |
| MonthFromEndMmm | `58` | Contohnya adalah M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Contohnya adalah Bulan 2, Bulan 1, Bulan -1, Bulan -2 |
| MonthFromStartMm | `61` | Contohnya adalah -2, -2, 1, 2 bulan sejak proyek dimulai. |
| MonthFromStartMmm | `60` | Contohnya adalah M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Contohnya Bulan -2, Bulan -1, Bulan 1, Bulan 2 |
| QuarterQ | `62` | Contohnya adalah 3, 4, 1. Membutuhkan satuan waktu menjadi TimescaleQuarters. |
| QuarterQq | `6` | Contohnya adalah Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Contohnya adalah Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Contohnya adalah Kuartal ke-3, Kuartal ke-1 |
| QuarterQQyy | `51` | Contohnya adalah 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Contohnya adalah Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Contohnya adalah Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Contohnya adalah 5, 4, 3, 2, 1, -1 kuartal dari akhir proyek. |
| QuarterFromEndQq | `63` | Contohnya adalah Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Contohnya adalah Kuartal 5, Kuartal 4, Kuartal 3, Kuartal 2, Kuartal 1, Kuartal -1 |
| QuarterFromStartQ | `66` | Contohnya adalah -5, -4, -3, -2, -1, 1 kuartal dari awal proyek. |
| QuarterFromStartQq | `65` | Contohnya adalah Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Contohnya adalah Kuartal -5, Kuartal -4, Kuartal -3, Kuartal -2, Kuartal -1, Kuartal 1 |
| ThirdsOfMonthsDd | `136` | Contohnya adalah 1, 11, 21, 1. Membutuhkan satuan waktu TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Contohnya adalah B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Contohnya adalah Awal, Tengah, Akhir, Awal |
| ThirdsOfMonthsMmDd | `139` | Contoh 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Contoh 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Contohnya adalah 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Contohnya adalah 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Contohnya adalah 1 Mar, 11 Mar, 21 Mar, 1 Apr |
| ThirdsOfMonthsMmmDdYy | `147` | Contohnya adalah Mar 1, '10; 11 Maret '10; 21 Maret '10; 1 Apr 10_x000h_ |
| ThirdsOfMonthsMmmDdd | `143` | Contohnya adalah Mar B, Mar M, Mar E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Contohnya adalah Mar B, '10; Mar M, '10; Maret E, '10; Apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Contohnya adalah 1 Maret, 11 Maret, 21 Maret, 1 April |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Contohnya adalah 1 Maret 2010; 11 Maret 2010; 21 Maret 2010; 1 April 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Contohnya adalah Awal Maret, Pertengahan Maret, Akhir Maret, Awal April |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Contohnya adalah Awal Maret 2010; Maret Tengah, 2010; Akhir Maret 2010; Awal April, 2010 |
| WeekDddDd | `88` | Contohnya adalah Sun 21, Sun 28, Sun 4. Memerlukan satuan waktu TimescaleWeeks. |
| WeekDddMDd | `97` | Contohnya adalah Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | Contohnya adalah Sun 3/21, Sun 3/28, Sun 4/4 |
| WeekDddMmDdYy | `100` | Contohnya adalah Sun 3/21/10, Sun 3/28/10, Sun 4/4/10 |
| WeekDddMmmDd | `93` | Contohnya adalah Minggu 21 Mar, Minggu 28 Maret, Minggu Apr 4 |
| WeekDddMmmDdYyy | `101` | Contohnya adalah Sun Mar 21, '10; Minggu 28 Maret '10; Minggu 4 Apr '10 |
| WeekDddMmmmDd | `96` | Contohnya adalah Minggu 21 Mar, Minggu 28 Maret, Minggu Apr 4 |
| WeekDddMmmmDdYyy | `102` | Contohnya adalah Minggu 21 Maret '10; Minggu 28 Maret '10; Minggu 4 April '10 |
| WeekDddWw | `103` | Contohnya adalah Matahari 12, Matahari 13, Matahari 14 |
| WeekDdiMDd | `98` | Contohnya adalah Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Contohnya adalah Su 3/21. Su 3/28, Su 4/4 |
| WeekDdiMmmDd | `94` | Contohnya adalah Su Mar 21, Su Mar 28, Su Apr 4 |
| WeekDiMDd | `99` | Contohnya adalah SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Contohnya adalah S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Contohnya adalah S 21 Mar, S 28 Mar, S Apr 4 |
| WeekMDd | `89` | Contohnya adalah M21, M28, A 4 |
| WeekMmDd | `17` | Contohnya adalah 21/3, 28/3, 4/4 |
| WeekMmDdYy | `16` | Contohnya adalah '3/21/10'. |
| WeekMmmDd | `15` | Contohnya adalah Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | Contohnya adalah Mar 21, '10; 28 Maret '10; 4 April '10 |
| WeekMmmmDd | `14` | Contohnya adalah 21 Maret, 28 Maret, 4 April |
| WeekMmmmDdYyyy | `12` | Contohnya adalah 21 Maret 2010; 28 Maret 2010; 4 April 2010 |
| WeekDayOfMonthDd | `87` | Contohnya adalah 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Contohnya adalah Minggu ke-2, Minggu ke-1, Minggu -1 dari akhir proyek. |
| WeekFromEndWw | `68` | Contohnya adalah 2, 1, -1 |
| WeekFromEndWww | `67` | Contohnya adalah W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Contohnya adalah Minggu -1, Minggu 1, Minggu 2 sejak proyek dimulai. |
| WeekFromStartWw | `70` | Contohnya adalah -1, 1, 2 |
| WeekFromStartWww | `69` | Contohnya adalah W-1, W1, W2 |
| WeekNumberDdWw | `104` | Contohnya adalah 1 12, 1 13, 1 14 (hari 1 minggu 12, hari 1 minggu 13, dan seterusnya) |
| WeekNumberWw | `50` | Contohnya adalah 12, 13, 14 |
| YearYy | `75` | Contohnya adalah 10, 11, 12. Membutuhkan satuan waktu berupa TimescaleYears. |
| YearYyy | `1` | Contohnya adalah '10, '11, '12 |
| YearYyyy | `0` | Contohnya adalah 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Contohnya adalah Tahun 2, Tahun 1, Tahun -1 dari akhir proyek. |
| YearFromEndYy | `72` | Contohnya adalah 2, 1, -1 |
| YearFromEndYyy | `71` | Contohnya adalah Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Contohnya adalah Tahun -1, Tahun 1, Tahun 2 dari awal proyek. |
| YearFromStartYy | `74` | Contohnya adalah -1, 1, 2 |
| YearFromStartYyy | `73` | Contohnya adalah Y-1, Y1, Y2 |

### Lihat juga

* ruang nama [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* perakitan [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
