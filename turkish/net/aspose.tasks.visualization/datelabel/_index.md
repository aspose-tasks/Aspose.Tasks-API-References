---
title: Enum DateLabel
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.Visualization.DateLabel Sıralama. Bir zaman ölçeğinde tarih ve saat etiketleri için görüntüleme formatını belirtir.
type: docs
weight: 2650
url: /tr/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Bir zaman ölçeğinde tarih ve saat etiketleri için görüntüleme formatını belirtir.

```csharp
public enum DateLabel
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| None | `35` | Tarih görüntülenmiyor. |
| DayDdd | `19` | Örnekler Pzt, Sal. |
| DayDddDd | `105` | Örnekler 30 Pzt, Sal 1 |
| DayDddMDd | `112` | Örnekler Pzt S 30, Sal O 1 |
| DayDddMmDd | `108` | Örnekler, Pzt 9/30, Sal 10/1 |
| DayDddMmDdYy | `52` | Örnekler 30/9/02 Pzt, 10/1/02 Sal |
| DayDddMmmDd | `23` | Örnekler 30 Eylül Pzt, 1 Ekim Sal |
| DayDddMmmDdYyy | `22` | Örnekler: 30 Eylül '02 Pzt, 1 Ekim '02 Sal |
| DayDddMmmmDd | `111` | Örnekler 30 Eylül Pzt, 1 Ekim Sal |
| DayDddd | `18` | Örnekler Salı, Çarşamba. |
| DayDdi | `119` | Örnekler: Mo, Tu |
| DayDdiDd | `106` | Örnekler Mo 30, Tu 1 |
| DayDdiMDd | `113` | Örnekler Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Örnekler Pzt 9/30, Sal 10/1 |
| DayDi | `20` | Örnekler M, T |
| DayDiDdSpace | `107` | Örnekler M 30, T 1 |
| DayDiMDd | `114` | Örnekler MS 30, TO 1 |
| DayDiMmDd | `110` | Örnekler M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Örnekler M30, T1 |
| DayMDd | `115` | Örnekler: S 30, O 1 |
| DayMmDd | `27` | Örnekler 9/30, 10/1 |
| DayMmDdYy | `26` | Örnekler 30/9/02, 1/10/02 |
| DayMmmDd | `25` | Örnekler 30 Eylül, 1 Ekim'dir |
| DayMmmDdYyy | `24` | Örnekler: 30 Eyl '02, 10 Eki '02 |
| DayFromEndDayDd | `41` | Örnekler, proje bitiminden itibaren 2. Gün, 1. Gün, -1. Gün, -2. Gün'dür. |
| DayFromEndDd | `54` | Örnekler: 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Örnekler: D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Örnekler, proje başlangıcından itibaren -2. Gün, -1. Gün, 1. Gün, 2. Gün'dür. |
| DayFromStartDd | `56` | Örnekler -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Örnekler: D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Örnekler 30, 1 |
| DayOfYearDd | `118` | Örnekler: 77, 78 |
| DayOfYearDdYyy | `116` | Örnekler: 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Örnekler: 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Örnek 19/07/2016. |
| HalfYearH | `128` | Örnekler 1, 2'dir. Zaman biriminin Zaman ÖlçeğiYarıYıl olmasını gerektirir. |
| HalfYearHh | `127` | Örnekler: H1, H2 |
| HalfYearHhYyy | `126` | Örnekler: H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Örnekler 1. Yarı, 2. Yarı |
| HalfYearHHyy | `129` | Örnekler: 1H10, 2H10 |
| HalfYearHlfH | `125` | Örnekler: Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Örnekler 1. Yarı, 2010; Yarı 2, 2010 |
| HalfYearFromEndH | `135` | Örnekler 2, 1, -1, -2'dir. Proje bitiş tarihinden itibaren yarım yıl. |
| HalfYearFromEndHalfH | `133` | Örnekler: Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Örnekler: H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Örnekler -2, -1, 1, 2'dir. Proje başlangıç tarihinden itibaren yarım yıl. |
| HalfYearFromStartHalfH | `130` | Örnekler Yarım -2, Yarım -1, Yarım 1, Yarım 2 |
| HalfYearFromStartHh | `131` | Örnekler: H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Örnekler: 18 Mart Çar, 08:00; Çar 18 Mart, 09:00. Zaman biriminin TimescaleHours. olmasını gerektirir |
| HourHh | `32` | Örnekler: 8, 9, 10, 11 |
| HourHhMmAm | `30` | Örnekler: 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Örnekler: 08:00, 09:00 |
| HourMmDdHhAm | `120` | Örnekler: 18/3 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Örnekler, 18 Mart, 08:00; 18 Mart 09:00 |
| HourFromEndHh | `77` | Örnekler, proje bitiminden itibaren 3, 2, 1, -1, -2 saattir. |
| HourFromEndHhh | `76` | Örnekler: H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Örnekler: Saat 3, Saat 2, Saat 1, Saat -1, Saat -2 |
| HourFromStartHh | `79` | Örnekler, proje başlangıcından itibaren -2, -1, 1, 2, 3 saattir. |
| HourFromStartHhh | `78` | Örnekler: H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Örnekler: Saat -2, Saat -1, Saat 1, Saat 2, Saat 3 |
| MinuteHhMmAm | `33` | Örnekler, 8:00 AM, 8:01 AM, 8:02 AM'dir. Zaman biriminin TimescaleMinutes. olmasını gerektirir |
| MinuteMm | `34` | Örnekler: 0, 1, 2, ..., 59 dakika |
| MinuteFromEndMinuteMm | `37` | Örnekler, proje bitiminden itibaren Dakika 181, Dakika 180, ..., Dakika 1, Dakika -1'dir. |
| MinuteFromEndMm | `81` | Örnekler: 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Örnekler şunlardır: M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Örnekler: Dakika -2, Dakika -1, Dakika 1, ... Proje başlangıcından itibaren Dakika 180. |
| MinuteFromStartMm | `83` | Örnekler -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Örnekler: M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Örnekler M, A, M, J, J'dir. Zaman biriminin TimescaleMonths. olmasını gerektirir. |
| MonthMm | `57` | Örnekler: 11, 12, 1, 2 |
| MonthMmYy | `86` | Örnekler: 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Örnekler: 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Örnekler: Mar, Nis, May |
| MonthMmmYyy | `8` | Örnekler: Mar '10, Nis '10, May '10 |
| MonthMmmm | `9` | Örnekler Mart, Nisan, Mayıs |
| MonthMmmmYyyy | `7` | Örnekler Mart 2010, Nisan 2010, Mayıs 2010 |
| MonthFromEndMm | `59` | Örnekler, proje bitiminden itibaren 2, 1, -1, -2 aydır. |
| MonthFromEndMmm | `58` | Örnekler: M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Örnekler: 2. Ay, 1. Ay, -1 Ay, -2 Ay |
| MonthFromStartMm | `61` | Örnekler, proje başlangıcından itibaren -2, -2, 1, 2 aydır. |
| MonthFromStartMmm | `60` | Örnekler: M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Örnekler: Ay -2, Ay -1, Ay 1, Ay 2 |
| QuarterQ | `62` | Örnekler 3, 4, 1'dir. Zaman biriminin TimescaleQuarters. olmasını gerektirir. |
| QuarterQq | `6` | Örnekler: Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Örnekler: Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Örnekler 3. Çeyrek, 1. Çeyrek |
| QuarterQQyy | `51` | Örnekler: 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Örnekler: Çey3, Çey4, Çey1 |
| QuarterQtrQYyyy | `3` | Örnekler, 3. Çeyrek, 2010; 4Ç 2010; Çey1, 2011 |
| QuarterFromEndQ | `64` | Örnekler, proje bitiminden itibaren 5, 4, 3, 2, 1, -1 çeyreklerdir. |
| QuarterFromEndQq | `63` | Örnekler: Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Örnekler, Çeyrek 5, Çeyrek 4, Çeyrek 3, Çeyrek 2, Çeyrek 1, Çeyrek -1 |
| QuarterFromStartQ | `66` | Örnekler, proje başlangıcından itibaren -5, -4, -3, -2, -1, 1 çeyreklerdir. |
| QuarterFromStartQq | `65` | Örnekler: Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Örnekler, Çeyrek -5, Çeyrek -4, Çeyrek -3, Çeyrek -2, Çeyrek -1, Çeyrek 1 |
| ThirdsOfMonthsDd | `136` | Örnekler 1, 11, 21, 1'dir. Zaman biriminin TimescaleThirdsOfMonths. olmasını gerektirir. |
| ThirdsOfMonthsDdd | `137` | Örnekler: B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Örnekler: Başlangıç, Orta, Bitiş, Başlangıç |
| ThirdsOfMonthsMmDd | `139` | Örnek: 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Örnek 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Örnekler: 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Örnek: 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Örnekler: 1 Mart, 11 Mart, 21 Mart, 1 Nisan |
| ThirdsOfMonthsMmmDdYy | `147` | Örnekler 1 Mar, '10; 11 Mart '10; 21 Mart '10; 1 Nisan 10 |
| ThirdsOfMonthsMmmDdd | `143` | Örnekler: Mar B, Mar M, Mar E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Örnekler Mar B, '10; Mar M, '10; Mar E, '10; Nis B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Örnekler 1 Mart, 11 Mart, 21 Mart, 1 Nisan'dır |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Örnekler 1 Mart 2010; 11 Mart 2010; 21 Mart 2010; 1 Nisan 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Örnekler Mart Başlangıcı, Mart Ortası, Mart Sonu, Nisan Başlangıcı |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Örnekler Mart Başlangıcı, 2010; Mart Ortası, 2010; Mart Sonu, 2010; Nisan Başlangıcı, 2010 |
| WeekDddDd | `88` | Örnekler, Paz 21, Paz 28, Paz 4'tür. Zaman biriminin TimescaleWeeks olmasını gerektirir. |
| WeekDddMDd | `97` | Örnekler: Güneş M 21, Güneş M 28, Güneş A 4 |
| WeekDddMmDd | `90` | Örnekler, Paz 3/21, Paz 3/28, Paz 4/4 |
| WeekDddMmDdYy | `100` | Örnekler 21/3/10 Paz, 28/3/10 Paz, 4/4/10 Paz |
| WeekDddMmmDd | `93` | Örnekler: 21 Mart Paz, 28 Mart Paz, 4 Nisan Paz |
| WeekDddMmmDdYyy | `101` | Örnekler Paz Mar 21, '10; Paz 28 Mar, '10; 4 Nis Paz, '10 |
| WeekDddMmmmDd | `96` | Örnekler: 21 Mart Paz, 28 Mart Paz, 4 Nisan Paz |
| WeekDddMmmmDdYyy | `102` | Örnekler, Paz Mart 21, '10; 28 Mart '10 Paz; 4 Nisan Paz '10 |
| WeekDddWw | `103` | Örnekler: Güneş 12, Güneş 13, Güneş 14 |
| WeekDdiMDd | `98` | Örnekler şunlardır: Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Örnekler Su 3/21'dir. Pa 3/28, Pa 4/4 |
| WeekDdiMmmDd | `94` | Örnekler: 21 Mart Paz, 28 Mart Pa, 4 Nisan Paz |
| WeekDiMDd | `99` | Örnekler: SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Örnekler: S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Örnekler: 21 Mart, 28 Mart, 4 Nisan |
| WeekMDd | `89` | Örnekler M21, M28, A 4 |
| WeekMmDd | `17` | Örnekler: 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Örnek '3/21/10'. |
| WeekMmmDd | `15` | Örnekler 21 Mart, 28 Mart, 4 Nisan'dır |
| WeekMmmDdYyy | `13` | Örnekler 21 Mar, '10; 28 Mart '10; 4 Nis, '10 |
| WeekMmmmDd | `14` | Örnekler 21 Mart, 28 Mart, 4 Nisan'dır |
| WeekMmmmDdYyyy | `12` | Örnekler 21 Mart 2010; 28 Mart 2010; 4 Nisan 2010 |
| WeekDayOfMonthDd | `87` | Örnekler: 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Örnekler, proje sonundan itibaren 2. Hafta, 1. Hafta, Hafta -1'dir. |
| WeekFromEndWw | `68` | Örnekler: 2, 1, -1 |
| WeekFromEndWww | `67` | Örnekler: W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Örnekler, proje başlangıcından itibaren Hafta -1, Hafta 1, Hafta 2'dir. |
| WeekFromStartWw | `70` | Örnekler -1, 1, 2 |
| WeekFromStartWww | `69` | Örnekler: W-1, W1, W2 |
| WeekNumberDdWw | `104` | Örnekler: 1 12, 1 13, 1 14 (12. haftanın 1. günü, 13. haftanın 1. günü vb.) |
| WeekNumberWw | `50` | Örnekler: 12, 13, 14 |
| YearYy | `75` | Örnekler 10, 11, 12'dir. Zaman biriminin TimescaleYears olmasını gerektirir. |
| YearYyy | `1` | Örnekler '10, '11, '12 'dir. |
| YearYyyy | `0` | Örnekler 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Örnekler, proje sonundan itibaren Yıl 2, Yıl 1, Yıl -1'dir. |
| YearFromEndYy | `72` | Örnekler: 2, 1, -1 |
| YearFromEndYyy | `71` | Örnekler Y2, Y1, Y-1 'dir. |
| YearFromStartYearYy | `48` | Örnekler, proje başlangıcından itibaren Yıl -1, Yıl 1, Yıl 2'dir. |
| YearFromStartYy | `74` | Örnekler -1, 1, 2 |
| YearFromStartYyy | `73` | Örnekler: Y-1, Y1, Y2 |

### Ayrıca bakınız

* ad alanı [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* toplantı [Aspose.Tasks](../../)


