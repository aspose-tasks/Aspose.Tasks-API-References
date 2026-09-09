---
title: "Enum DateLabel"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.DateLabel enum. Zaman ölçeğinde tarih ve saat etiketlerinin görüntüleme biçimini belirtir"
type: docs
weight: 2980
url: /tr/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Zaman ölçeğindeki tarih ve saat etiketleri için görüntüleme biçimini belirtir.

```csharp
public enum DateLabel
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `35` | Tarih görüntülenmez. |
| DayDdd | `19` | Örnekler: Paz, Sal. |
| DayDddDd | `105` | Örnekler: Paz 30, Sal 1 |
| DayDddMDd | `112` | Örnekler: Paz S 30, Sal O 1 |
| DayDddMmDd | `108` | Örnekler: Paz 9/30, Sal 10/1 |
| DayDddMmDdYy | `52` | Örnekler: Paz 9/30/02, Sal 10/1/02 |
| DayDddMmmDd | `23` | Örnekler: Paz Sep 30, Sal Oct 1 |
| DayDddMmmDdYyy | `22` | Örnekler: Paz Sep 30 '02, Sal Oct 1 '02 |
| DayDddMmmmDd | `111` | Örnekler: Paz Eylül 30, Sal Ekim 1 |
| DayDddd | `18` | Örnekler: Salı, Çarşamba. |
| DayDdi | `119` | Örnekler: Pzt, Sal |
| DayDdiDd | `106` | Örnekler: Pzt 30, Sal 1 |
| DayDdiMDd | `113` | Örnekler: Pzt S 30, Sal O 1 |
| DayDdiMmDd | `109` | Örnekler: Pzt 9/30, Sal 10/1 |
| DayDi | `20` | Örnekler: P, S |
| DayDiDdSpace | `107` | Örnekler: P 30, S 1 |
| DayDiMDd | `114` | Örnekler: P S 30, S O 1 |
| DayDiMmDd | `110` | Örnekler: P 9/30, S 10/1 |
| DayDiDdNoSpace | `121` | Örnekler: P30, S1 |
| DayMDd | `115` | Örnekler: S 30, O 1 |
| DayMmDd | `27` | Örnekler: 9/30, 10/1 |
| DayMmDdYy | `26` | Örnekler: 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Örnekler Sep 30, Oct 1 |
| DayMmmDdYyy | `24` | Örnekler Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | Örnekler Day 2, Day 1, Day -1, Day -2 proje sonundan. |
| DayFromEndDd | `54` | Örnekler 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Örnekler D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Örnekler Day -2, Day -1, Day 1, Day 2 proje başlangıcından. |
| DayFromStartDd | `56` | Örnekler -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Örnekler D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Örnekler 30, 1 |
| DayOfYearDd | `118` | Örnekler 77, 78 |
| DayOfYearDdYyy | `116` | Örnekler 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Örnekler 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Örnek 19/07/2016. |
| HalfYearH | `128` | Örnekler 1, 2. Zaman biriminin TimescaleHalfYears olması gerekir. |
| HalfYearHh | `127` | Örnekler H1, H2 |
| HalfYearHhYyy | `126` | Örnekler H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Örnekler 1st Half, 2d Half |
| HalfYearHHyy | `129` | Örnekler 1H10, 2H10 |
| HalfYearHlfH | `125` | Örnekler Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Örnekler Half 1, 2010; Half 2, 2010 |
| HalfYearFromEndH | `135` | Örnekler 2, 1, -1, -2. Proje bitiş tarihinden yarım yıllar. |
| HalfYearFromEndHalfH | `133` | Örnekler Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Örnekler H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Örnekler -2, -1, 1, 2. Proje başlangıç tarihinden yarım yıllar. |
| HalfYearFromStartHalfH | `130` | Örnekler Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Örnekler H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Örnekler Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Zaman biriminin TimescaleHours olması gerekir. |
| HourHh | `32` | Örnekler 8, 9, 10, 11 |
| HourHhMmAm | `30` | Örnekler 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Örnekler 8AM, 9AM |
| HourMmDdHhAm | `120` | Örnekler 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Örnekler Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | Örnekler proje sonundan 3, 2, 1, -1, -2 saat. |
| HourFromEndHhh | `76` | Örnekler H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Örnekler Saat 3, Saat 2, Saat 1, Saat -1, Saat -2 |
| HourFromStartHh | `79` | Örnekler proje başlangıcından -2, -1, 1, 2, 3 saat. |
| HourFromStartHhh | `78` | Örnekler H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Örnekler Saat -2, Saat -1, Saat 1, Saat 2, Saat 3 |
| MinuteHhMmAm | `33` | Örnekler 8:00 AM, 8:01 AM, 8:02 AM. Zaman biriminin TimescaleMinutes olması gerekir. |
| MinuteMm | `34` | Örnekler 0, 1, 2, ..., 59 dakika |
| MinuteFromEndMinuteMm | `37` | Örnekler proje sonundan Dakika 181, Dakika 180, ..., Dakika 1, Dakika -1. |
| MinuteFromEndMm | `81` | Örnekler 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Örnekler M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Örnekler proje başlangıcından Dakika -2, Dakika -1, Dakika 1, ... Dakika 180. |
| MinuteFromStartMm | `83` | Örnekler -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Örnekler M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Örnekler M, A, M, J, J. Zaman biriminin TimescaleMonths olması gerekir. |
| MonthMm | `57` | Örnekler 11, 12, 1, 2 |
| MonthMmYy | `86` | Örnekler 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Örnekler 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Örnekler Mar, Apr, May |
| MonthMmmYyy | `8` | Örnekler Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | Örnekler March, April, May |
| MonthMmmmYyyy | `7` | Örnekler March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | Örnekler 2, 1, -1, -2 ay proje sonundan. |
| MonthFromEndMmm | `58` | Örnekler M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Örnekler Month 2, Month 1, Month -1, Month -2 |
| MonthFromStartMm | `61` | Örnekler -2, -2, 1, 2 ay proje başlangıcından. |
| MonthFromStartMmm | `60` | Örnekler M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Örnekler Month -2, Month -1, Month 1, Month 2 |
| QuarterQ | `62` | Örnekler 3, 4, 1. Zaman biriminin TimescaleQuarters olması gerekir. |
| QuarterQq | `6` | Örnekler Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Örnekler Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Örnekler 3rd Quarter, 1st Quarter |
| QuarterQQyy | `51` | Örnekler 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Örnekler Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Örnekler Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Örnekler 5, 4, 3, 2, 1, -1 çeyrek proje sonundan. |
| QuarterFromEndQq | `63` | Örnekler Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Örnekler Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | Örnekler -5, -4, -3, -2, -1, 1 çeyrek proje başlangıcından. |
| QuarterFromStartQq | `65` | Örnekler Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Örnekler Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | Örnekler 1, 11, 21, 1. Zaman biriminin TimescaleThirdsOfMonths olması gerekir. |
| ThirdsOfMonthsDdd | `137` | Örnekler B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Örnekler Başlangıç, Orta, Son, Başlangıç |
| ThirdsOfMonthsMmDd | `139` | Örnek 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Örnek 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Örnekler 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Örnek 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Örnekler Mar 1, Mar 11, Mar 21, Apr 1 |
| ThirdsOfMonthsMmmDdYy | `147` | Örnekler Mar 1, '10; Mar 11, '10; Mar 21, '10; Apr 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Örnekler Mar B, Mar M, Mar E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Örnekler Mar B, '10; Mar M, '10; Mar E, '10; Apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Örnekler Mart 1, Mart 11, Mart 21, Nisan 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Örnekler Mart 1, 2010; Mart 11, 2010; Mart 21, 2010; Nisan 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Örnekler Mart Başlangıç, Mart Orta, Mart Son, Nisan Başlangıç |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Örnekler Mart Başlangıç, 2010; Mart Orta, 2010; Mart Son, 2010; Nisan Başlangıç, 2010 |
| WeekDddDd | `88` | Örnekler Paz 21, Paz 28, Paz 4. Zaman biriminin TimescaleWeeks olmasını gerektirir. |
| WeekDddMDd | `97` | Örnekler Paz M 21, Paz M 28, Paz A 4 |
| WeekDddMmDd | `90` | Örnekler Paz 3/21, Paz 3/28, Paz 4/4 |
| WeekDddMmDdYy | `100` | Örnekler Paz 3/21/10, Paz 3/28/10, Paz 4/4/10 |
| WeekDddMmmDd | `93` | Örnekler Paz Mart 21, Paz Mart 28, Paz Nisan 4 |
| WeekDddMmmDdYyy | `101` | Örnekler Paz Mart 21, '10; Paz Mart 28, '10; Paz Nisan 4, '10 |
| WeekDddMmmmDd | `96` | Örnekler Paz Mart 21, Paz Mart 28, Paz Nisan 4 |
| WeekDddMmmmDdYyy | `102` | Örnekler Paz Mart 21, '10; Paz Mart 28, '10; Paz Nisan 4, '10 |
| WeekDddWw | `103` | Örnekler Paz 12, Paz 13, Paz 14 |
| WeekDdiMDd | `98` | Örnekler Paz M 21, Paz M 28, Paz A 4 |
| WeekDdiMmDd | `91` | Örnekler Paz 3/21. Paz 3/28, Paz 4/4 |
| WeekDdiMmmDd | `94` | Örnekler Paz Mart 21, Paz Mart 28, Paz Nisan 4 |
| WeekDiMDd | `99` | Örnekler S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Örnekler S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Örnekler S Mar 21, S Mar 28, S Nis 4 |
| WeekMDd | `89` | Örnekler M21, M28, A 4 |
| WeekMmDd | `17` | Örnekler 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Örnek '3/21/10'. |
| WeekMmmDd | `15` | Örnekler Mar 21, Mar 28, Nis 4 |
| WeekMmmDdYyy | `13` | Örnekler Mar 21, '10; Mar 28, '10; Nis 4, '10 |
| WeekMmmmDd | `14` | Örnekler Mart 21, Mart 28, Nisan 4 |
| WeekMmmmDdYyyy | `12` | Örnekler Mart 21, 2010; Mart 28, 2010; Nisan 4, 2010 |
| WeekDayOfMonthDd | `87` | Örnekler 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Örnekler Hafta 2, Hafta 1, Hafta -1 proje sonundan. |
| WeekFromEndWw | `68` | Örnekler 2, 1, -1 |
| WeekFromEndWww | `67` | Örnekler W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Örnekler Hafta -1, Hafta 1, Hafta 2 proje başlangıcından. |
| WeekFromStartWw | `70` | Örnekler -1, 1, 2 |
| WeekFromStartWww | `69` | Örnekler W-1, W1, W2 |
| WeekNumberDdWw | `104` | Örnekler 1 12, 1 13, 1 14 (12 haftanın 1. günü, 13 haftanın 1. günü, ve benzeri) |
| WeekNumberWw | `50` | Örnekler 12, 13, 14 |
| YearYy | `75` | Örnekler 10, 11, 12. Zaman biriminin TimescaleYears olması gerekir. |
| YearYyy | `1` | Örnekler '10, '11, '12 |
| YearYyyy | `0` | Örnekler 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Örnekler Yıl 2, Yıl 1, Yıl -1 proje sonundan. |
| YearFromEndYy | `72` | Örnekler 2, 1, -1 |
| YearFromEndYyy | `71` | Örnekler Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Örnekler Yıl -1, Yıl 1, Yıl 2 proje başlangıcından. |
| YearFromStartYy | `74` | Örnekler -1, 1, 2 |
| YearFromStartYyy | `73` | Örnekler Y-1, Y1, Y2 |

## Örnekler

Zaman ölçeği katman etiketlerini nasıl özelleştireceğinizi gösterir.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Görev bağlantılarını ekle
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// zaman ölçeği katmanlarını ayarla

// üst katmanı ayarla
// Gantt Şeması görünümünün üst zaman ölçeği katmanını ayarla.
view.MiddleTimescaleTier = new TimescaleTier();
// Zaman ölçeği katmanı için zaman ölçeği birimini <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> ayarla.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// Katman için etiketlerin gösterileceği zaman birimi aralığını ayarla.
view.MiddleTimescaleTier.Count = 1;
// Zaman ölçeği katmanı için tarih etiketini <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> ayarla.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını ayarla (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// katmanda zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değer ayarlayın.
view.MiddleTimescaleTier.ShowTicks = true;
// katman etiketlerini mali yıla dayandırıp dayandırmayacağını belirten bir değer ayarlayın.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// daha iyi görselleştirme için eklendi
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// orta katman tarihlerini özelleştirin
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Görünümde tanımlanan zaman ölçeği ayarlarını (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier) kullanarak zaman ölçeklerini oluşturmak için 'Timescale.DefinedInView' seçeneğini kullanın.
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


