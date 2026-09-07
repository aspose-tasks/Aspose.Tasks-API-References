---
title: "Απαρίθμηση DateLabel"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Visualization.DateLabel. Καθορίζει τη μορφή εμφάνισης ετικετών ημερομηνίας και ώρας σε κλίμακα χρόνου"
type: docs
weight: 2980
url: /el/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Καθορίζει τη μορφή εμφάνισης για ετικέτες ημερομηνίας και ώρας σε κλίμακα χρόνου.

```csharp
public enum DateLabel
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `35` | Δεν εμφανίζεται ημερομηνία. |
| DayDdd | `19` | Παραδείγματα: Δευ, Τρι. |
| DayDddDd | `105` | Παραδείγματα: Δευ 30, Τρι 1 |
| DayDddMDd | `112` | Παραδείγματα: Δευ S 30, Τρι O 1 |
| DayDddMmDd | `108` | Παραδείγματα: Δευ 9/30, Τρι 10/1 |
| DayDddMmDdYy | `52` | Παραδείγματα: Δευ 9/30/02, Τρι 10/1/02 |
| DayDddMmmDd | `23` | Παραδείγματα: Δευ Σεπ 30, Τρι Οκτ 1 |
| DayDddMmmDdYyy | `22` | Παραδείγματα: Δευ Σεπ 30 '02, Τρι Οκτ 1 '02 |
| DayDddMmmmDd | `111` | Παραδείγματα: Δευ Σεπτέμβριος 30, Τρι Οκτώβριος 1 |
| DayDddd | `18` | Παραδείγματα: Τρίτη, Τετάρτη. |
| DayDdi | `119` | Παραδείγματα: Δε, Τρ |
| DayDdiDd | `106` | Παραδείγματα: Δε 30, Τρ 1 |
| DayDdiMDd | `113` | Παραδείγματα: Δε S 30, Τρ O 1 |
| DayDdiMmDd | `109` | Παραδείγματα: Δε 9/30, Τρ 10/1 |
| DayDi | `20` | Παραδείγματα: Δ, Τ |
| DayDiDdSpace | `107` | Παραδείγματα: Δ 30, Τ 1 |
| DayDiMDd | `114` | Παραδείγματα: Δ S 30, Τ O 1 |
| DayDiMmDd | `110` | Παραδείγματα: Δ 9/30, Τ 10/1 |
| DayDiDdNoSpace | `121` | Παραδείγματα: Δ30, Τ1 |
| DayMDd | `115` | Παραδείγματα: S 30, O 1 |
| DayMmDd | `27` | Παραδείγματα: 9/30, 10/1 |
| DayMmDdYy | `26` | Παραδείγματα: 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Τα παραδείγματα είναι Σεπ 30, Οκτ 1 |
| DayMmmDdYyy | `24` | Τα παραδείγματα είναι Σεπ 30 '02, Οκτ 10 '02 |
| DayFromEndDayDd | `41` | Τα παραδείγματα είναι Ημέρα 2, Ημέρα 1, Ημέρα -1, Ημέρα -2 από το τέλος του έργου. |
| DayFromEndDd | `54` | Τα παραδείγματα είναι 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Τα παραδείγματα είναι D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Τα παραδείγματα είναι Ημέρα -2, Ημέρα -1, Ημέρα 1, Ημέρα 2 από την έναρξη του έργου. |
| DayFromStartDd | `56` | Τα παραδείγματα είναι -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Τα παραδείγματα είναι D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Τα παραδείγματα είναι 30, 1 |
| DayOfYearDd | `118` | Τα παραδείγματα είναι 77, 78 |
| DayOfYearDdYyy | `116` | Τα παραδείγματα είναι 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Τα παραδείγματα είναι 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Το παράδειγμα είναι 19/07/2016. |
| HalfYearH | `128` | Τα παραδείγματα είναι 1, 2. Απαιτεί η μονάδα χρόνου να είναι TimescaleHalfYears. |
| HalfYearHh | `127` | Τα παραδείγματα είναι H1, H2 |
| HalfYearHhYyy | `126` | Τα παραδείγματα είναι H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Τα παραδείγματα είναι 1ο Ημισύ, 2ο Ημισύ |
| HalfYearHHyy | `129` | Τα παραδείγματα είναι 1H10, 2H10 |
| HalfYearHlfH | `125` | Τα παραδείγματα είναι Ημισυ 1, Ημισυ 2 |
| HalfYearHlfHYyyy | `124` | Τα παραδείγματα είναι Ημισυ 1, 2010; Ημισυ 2, 2010 |
| HalfYearFromEndH | `135` | Τα παραδείγματα είναι 2, 1, -1, -2. Ημιετηρίες από την ημερομηνία λήξης του έργου. |
| HalfYearFromEndHalfH | `133` | Τα παραδείγματα είναι Ημισυ 2, Ημισυ 1, Ημισυ -1, Ημισυ -2 |
| HalfYearFromEndHh | `134` | Τα παραδείγματα είναι H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Τα παραδείγματα είναι -2, -1, 1, 2. Ημιετηρίες από την ημερομηνία έναρξης του έργου. |
| HalfYearFromStartHalfH | `130` | Τα παραδείγματα είναι Ημισυ -2, Ημισυ -1, Ημισυ 1, Ημισυ 2 |
| HalfYearFromStartHh | `131` | Παραδείγματα είναι H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Παραδείγματα είναι Wed Mar 18, 8 π.μ.; Wed Mar 18, 9 π.μ. Απαιτείται η μονάδα χρόνου να είναι TimescaleHours. |
| HourHh | `32` | Παραδείγματα είναι 8, 9, 10, 11 |
| HourHhMmAm | `30` | Παραδείγματα είναι 8:00 π.μ., 9:00 π.μ. |
| HourHhAm | `31` | Παραδείγματα είναι 8π.μ., 9π.μ. |
| HourMmDdHhAm | `120` | Παραδείγματα είναι 3/18 8 π.μ., 3/18 9 π.μ. |
| HourMmmDdHhAm | `29` | Παραδείγματα είναι Mar 18, 8 π.μ.; Mar 18, 9 π.μ. |
| HourFromEndHh | `77` | Παραδείγματα είναι 3, 2, 1, -1, -2 ώρες από το τέλος του έργου. |
| HourFromEndHhh | `76` | Παραδείγματα είναι H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Παραδείγματα είναι Ώρα 3, Ώρα 2, Ώρα 1, Ώρα -1, Ώρα -2 |
| HourFromStartHh | `79` | Παραδείγματα είναι -2, -1, 1, 2, 3 ώρες από την έναρξη του έργου. |
| HourFromStartHhh | `78` | Παραδείγματα είναι H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Παραδείγματα είναι Ώρα -2, Ώρα -1, Ώρα 1, Ώρα 2, Ώρα 3 |
| MinuteHhMmAm | `33` | Παραδείγματα είναι 8:00 π.μ., 8:01 π.μ., 8:02 π.μ. Απαιτείται η μονάδα χρόνου να είναι TimescaleMinutes. |
| MinuteMm | `34` | Παραδείγματα είναι 0, 1, 2, ..., 59 λεπτά |
| MinuteFromEndMinuteMm | `37` | Παραδείγματα είναι Λεπτό 181, Λεπτό 180, ..., Λεπτό 1, Λεπτό -1 από το τέλος του έργου. |
| MinuteFromEndMm | `81` | Παραδείγματα είναι 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Παραδείγματα είναι M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Παραδείγματα είναι Λεπτό -2, Λεπτό -1, Λεπτό 1, ... Λεπτό 180 από την έναρξη του έργου. |
| MinuteFromStartMm | `83` | Παραδείγματα είναι -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Παραδείγματα είναι M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Παραδείγματα είναι M, A, M, J, J. Απαιτείται η μονάδα χρόνου να είναι TimescaleMonths. |
| MonthMm | `57` | Παραδείγματα είναι 11, 12, 1, 2 |
| MonthMmYy | `86` | Παραδείγματα είναι 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Παραδείγματα είναι 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Παραδείγματα είναι Mar, Apr, May |
| MonthMmmYyy | `8` | Παραδείγματα είναι Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | Παραδείγματα είναι March, April, May |
| MonthMmmmYyyy | `7` | Παραδείγματα είναι March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | Παραδείγματα είναι 2, 1, -1, -2 μήνες από το τέλος του έργου. |
| MonthFromEndMmm | `58` | Παραδείγματα είναι M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Παραδείγματα είναι Μήνας 2, Μήνας 1, Μήνας -1, Μήνας -2 |
| MonthFromStartMm | `61` | Παραδείγματα είναι -2, -2, 1, 2 μήνες από την έναρξη του έργου. |
| MonthFromStartMmm | `60` | Παραδείγματα είναι M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Παραδείγματα είναι Μήνας -2, Μήνας -1, Μήνας 1, Μήνας 2 |
| QuarterQ | `62` | Παραδείγματα είναι 3, 4, 1. Απαιτείται η μονάδα χρόνου να είναι TimescaleQuarters. |
| QuarterQq | `6` | Παραδείγματα είναι Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Παραδείγματα είναι Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Παραδείγματα είναι 3ο Τρίμηνο, 1ο Τρίμηνο |
| QuarterQQyy | `51` | Παραδείγματα είναι 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Παραδείγματα είναι Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Παραδείγματα είναι Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Παραδείγματα είναι 5, 4, 3, 2, 1, -1 τρίμηνα από το τέλος του έργου. |
| QuarterFromEndQq | `63` | Παραδείγματα είναι Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Παραδείγματα είναι Τρίμηνο 5, Τρίμηνο 4, Τρίμηνο 3, Τρίμηνο 2, Τρίμηνο 1, Τρίμηνο -1 |
| QuarterFromStartQ | `66` | Παραδείγματα είναι -5, -4, -3, -2, -1, 1 τρίμηνα από την έναρξη του έργου. |
| QuarterFromStartQq | `65` | Παραδείγματα είναι Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Παραδείγματα είναι Τρίμηνο -5, Τρίμηνο -4, Τρίμηνο -3, Τρίμηνο -2, Τρίμηνο -1, Τρίμηνο 1 |
| ThirdsOfMonthsDd | `136` | Παραδείγματα είναι 1, 11, 21, 1. Απαιτείται η μονάδα χρόνου να είναι TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Παραδείγματα είναι B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Τα παραδείγματα είναι Αρχή, Μέση, Τέλος, Αρχή |
| ThirdsOfMonthsMmDd | `139` | Το παράδειγμα είναι 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Το παράδειγμα είναι 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Τα παραδείγματα είναι 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Το παράδειγμα είναι 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Τα παραδείγματα είναι Μαρ 1, Μαρ 11, Μαρ 21, Απρ 1 |
| ThirdsOfMonthsMmmDdYy | `147` | Τα παραδείγματα είναι Μαρ 1, '10; Μαρ 11, '10; Μαρ 21, '10; Απρ 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Τα παραδείγματα είναι Μαρ B, Μαρ M, Μαρ E, Απρ B |
| ThirdsOfMonthsMmmDddYy | `148` | Τα παραδείγματα είναι Μαρ B, '10; Μαρ M, '10; Μαρ E, '10; Απρ B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Τα παραδείγματα είναι Μάρτιος 1, Μάρτιος 11, Μάρτιος 21, Απρίλιος 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Τα παραδείγματα είναι Μάρτιος 1, 2010; Μάρτιος 11, 2010; Μάρτιος 21, 2010; Απρίλιος 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Τα παραδείγματα είναι Μάρτιος Αρχή, Μάρτιος Μέση, Μάρτιος Τέλος, Απρίλιος Αρχή |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Τα παραδείγματα είναι Μάρτιος Αρχή, 2010; Μάρτιος Μέση, 2010; Μάρτιος Τέλος, 2010; Απρίλιος Αρχή, 2010 |
| WeekDddDd | `88` | Τα παραδείγματα είναι Κυρ 21, Κυρ 28, Κυρ 4. Απαιτείται η μονάδα χρόνου να είναι TimescaleWeeks. |
| WeekDddMDd | `97` | Τα παραδείγματα είναι Κυρ M 21, Κυρ M 28, Κυρ A 4 |
| WeekDddMmDd | `90` | Τα παραδείγματα είναι Κυρ 3/21, Κυρ 3/28, Κυρ 4/4 |
| WeekDddMmDdYy | `100` | Τα παραδείγματα είναι Κυρ 3/21/10, Κυρ 3/28/10, Κυρ 4/4/10 |
| WeekDddMmmDd | `93` | Τα παραδείγματα είναι Κυρ Μαρ 21, Κυρ Μαρ 28, Κυρ Απρ 4 |
| WeekDddMmmDdYyy | `101` | Τα παραδείγματα είναι Κυρ Μαρ 21, '10; Κυρ Μαρ 28, '10; Κυρ Απρ 4, '10 |
| WeekDddMmmmDd | `96` | Τα παραδείγματα είναι Κυρ Μαρ 21, Κυρ Μάρτιος 28, Κυρ Απρ 4 |
| WeekDddMmmmDdYyy | `102` | Τα παραδείγματα είναι Κυρ Μάρτιος 21, '10; Κυρ Μάρτιος 28, '10; Κυρ Απρίλιος 4, '10 |
| WeekDddWw | `103` | Τα παραδείγματα είναι Κυρ 12, Κυρ 13, Κυρ 14 |
| WeekDdiMDd | `98` | Τα παραδείγματα είναι Κυρ M 21, Κυρ M 28, Κυρ A 4 |
| WeekDdiMmDd | `91` | Τα παραδείγματα είναι Κυρ 3/21. Κυρ 3/28, Κυρ 4/4 |
| WeekDdiMmmDd | `94` | Τα παραδείγματα είναι Κυρ Μαρ 21, Κυρ Μαρ 28, Κυρ Απρ 4 |
| WeekDiMDd | `99` | Παραδείγματα είναι S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Παραδείγματα είναι S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Παραδείγματα είναι S Μαρ 21, S Μαρ 28, S Απρ 4 |
| WeekMDd | `89` | Παραδείγματα είναι M21, M28, A 4 |
| WeekMmDd | `17` | Παραδείγματα είναι 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Παράδειγμα είναι '3/21/10'. |
| WeekMmmDd | `15` | Παραδείγματα είναι Μαρ 21, Μαρ 28, Απρ 4 |
| WeekMmmDdYyy | `13` | Παραδείγματα είναι Μαρ 21, '10; Μαρ 28, '10; Απρ 4, '10 |
| WeekMmmmDd | `14` | Παραδείγματα είναι Μάρτιος 21, Μάρτιος 28, Απρίλιος 4 |
| WeekMmmmDdYyyy | `12` | Παραδείγματα είναι Μάρτιος 21, 2010; Μάρτιος 28, 2010; Απρίλιος 4, 2010 |
| WeekDayOfMonthDd | `87` | Παραδείγματα είναι 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Παραδείγματα είναι Εβδομάδα 2, Εβδομάδα 1, Εβδομάδα -1 από το τέλος του έργου. |
| WeekFromEndWw | `68` | Παραδείγματα είναι 2, 1, -1 |
| WeekFromEndWww | `67` | Παραδείγματα είναι W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Παραδείγματα είναι Εβδομάδα -1, Εβδομάδα 1, Εβδομάδα 2 από την έναρξη του έργου. |
| WeekFromStartWw | `70` | Παραδείγματα είναι -1, 1, 2 |
| WeekFromStartWww | `69` | Παραδείγματα είναι W-1, W1, W2 |
| WeekNumberDdWw | `104` | Παραδείγματα είναι 1 12, 1 13, 1 14 (ημέρα 1 της εβδομάδας 12, ημέρα 1 της εβδομάδας 13, και ούτω καθεξής) |
| WeekNumberWw | `50` | Παραδείγματα είναι 12, 13, 14 |
| YearYy | `75` | Παραδείγματα είναι 10, 11, 12. Απαιτείται η μονάδα χρόνου να είναι TimescaleYears. |
| YearYyy | `1` | Παραδείγματα είναι '10, '11, '12 |
| YearYyyy | `0` | Παραδείγματα είναι 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Παραδείγματα είναι Έτος 2, Έτος 1, Έτος -1 από το τέλος του έργου. |
| YearFromEndYy | `72` | Παραδείγματα είναι 2, 1, -1 |
| YearFromEndYyy | `71` | Παραδείγματα είναι Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Παραδείγματα είναι Έτος -1, Έτος 1, Έτος 2 από την έναρξη του έργου. |
| YearFromStartYy | `74` | Παραδείγματα είναι -1, 1, 2 |
| YearFromStartYyy | `73` | Τα παραδείγματα είναι Y-1, Y1, Y2 |

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τις ετικέτες του επιπέδου κλίμακας χρόνου.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Προσθήκη συνδέσμων εργασιών
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ρυθμίστε τα επίπεδα κλίμακας χρόνου

// ρυθμίστε το ανώτερο επίπεδο
// ορίστε το ανώτερο επίπεδο κλίμακας χρόνου της προβολής Διάγραμμα Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// ορίστε τη μονάδα κλίμακας χρόνου <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> για το επίπεδο κλίμακας χρόνου.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// ορίστε το διάστημα μονάδας χρόνου στο οποίο θα εμφανίζονται οι ετικέτες για το επίπεδο.
view.MiddleTimescaleTier.Count = 1;
// ορίστε την ετικέτα ημερομηνίας <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> για το επίπεδο κλίμακας χρόνου.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// ορίστε πώς θα ευθυγραμμιστούν οι ετικέτες εντός κάθε χρονικής περιόδου του επιπέδου (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζονται σημεία σήμανσης που χωρίζουν χρονικές περιόδους στο επίπεδο.
view.MiddleTimescaleTier.ShowTicks = true;
// ορίστε μια τιμή που υποδεικνύει εάν οι ετικέτες του επιπέδου θα βασίζονται στο οικονομικό έτος.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// προστέθηκε για καλύτερη απεικόνιση
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// προσαρμόστε τις ημερομηνίες του μεσαίου επιπέδου
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Χρησιμοποιήστε την επιλογή 'Timescale.DefinedInView' για την απόδοση των κλιμάκων χρόνου χρησιμοποιώντας τις ρυθμίσεις κλίμακας χρόνου που ορίζονται στην προβολή (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


