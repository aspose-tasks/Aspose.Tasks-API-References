---
title: DateLabel
second_title: Aspose.Tasks لمرجع .NET API
description: يحدد تنسيق العرض لملصقات التاريخ والوقت بمقياس زمني.
type: docs
weight: 2630
url: /ar/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

يحدد تنسيق العرض لملصقات التاريخ والوقت بمقياس زمني.

```csharp
public enum DateLabel
```

### قيم

| اسم | قيمة | وصف |
| --- | --- | --- |
| None | `35` | لا يوجد تاريخ معروض . |
| DayDdd | `19` | الأمثلة هي الاثنين ، الثلاثاء . |
| DayDddDd | `105` | من الأمثلة الاثنين 30 ، الثلاثاء 1 |
| DayDddMDd | `112` | الأمثلة هي Mon S 30 ، Tue O 1 |
| DayDddMmDd | `108` | الأمثلة هي الاثنين 9/30 ، الثلاثاء 10 / 1 |
| DayDddMmDdYy | `52` | الأمثلة هي الاثنين 30 9/02 ، الثلاثاء 10/1 / 02 |
| DayDddMmmDd | `23` | الأمثلة هي الاثنين 30 سبتمبر ، الثلاثاء أكتوبر 1 |
| DayDddMmmDdYyy | `22` | الأمثلة هي الاثنين سبتمبر 30 '02 ، الثلاثاء 1 أكتوبر '02 |
| DayDddMmmmDd | `111` | الأمثلة هي الاثنين 30 سبتمبر ، الثلاثاء 1 أكتوبر 1 |
| DayDddd | `18` | الأمثلة هي الثلاثاء والأربعاء . |
| DayDdi | `119` | الأمثلة هي Mo ، Tu |
| DayDdiDd | `106` | الأمثلة هي Mo 30 ، Tu 1 |
| DayDdiMDd | `113` | الأمثلة هي Mo S 30 ، Tu O 1 |
| DayDdiMmDd | `109` | الأمثلة هي Mo 9/30 ، Tu 10 / 1 |
| DayDi | `20` | الأمثلة M ، T |
| DayDiDdSpace | `107` | الأمثلة هي M 30 ، T 1 |
| DayDiMDd | `114` | الأمثلة هي MS 30 ، TO 1 |
| DayDiMmDd | `110` | الأمثلة M 9/30 ، T 10 / 1 |
| DayDiDdNoSpace | `121` | الأمثلة هي M30 ، T1 |
| DayMDd | `115` | الأمثلة هي S 30 ، O 1 |
| DayMmDd | `27` | الأمثلة هي 9/30 ، 10 / 1 |
| DayMmDdYy | `26` | الأمثلة هي 9/30/02 ، 10/1 / 02 |
| DayMmmDd | `25` | من الأمثلة 30 سبتمبر ، 1 أكتوبر |
| DayMmmDdYyy | `24` | الأمثلة هي 30 سبتمبر '02 ، 10 أكتوبر '02 |
| DayFromEndDayDd | `41` | الأمثلة هي اليوم 2 ، اليوم 1 ، اليوم -1 ، اليوم -2 من نهاية المشروع . |
| DayFromEndDd | `54` | الأمثلة هي 2 ، 1 ، -1 ، -2 |
| DayFromEndDdd | `53` | الأمثلة هي D2 و D1 و D-1 و D-2 |
| DayFromStartDayDd | `40` | الأمثلة هي اليوم -2 ، واليوم -1 ، واليوم 1 ، واليوم 2 من بداية المشروع . |
| DayFromStartDd | `56` | الأمثلة هي -2 ، -1 ، 1 ، 2 |
| DayFromStartDdd | `55` | الأمثلة هي D-2 و D-1 و D1 و D2 |
| DayOfMonthDd | `21` | الأمثلة هي 30 ، 1 |
| DayOfYearDd | `118` | الأمثلة هي 77 ، 78 |
| DayOfYearDdYyy | `116` | الأمثلة هي 77 '10 ، 78 '10 |
| DayOfYearDdYyyy | `117` | الأمثلة هي 77 2010 ، 78 2010 |
| DayDdMmYyyy | `256` | المثال هو 19/07/2016 . |
| HalfYearH | `128` | الأمثلة هي 1 ، 2. تتطلب أن تكون الوحدة الزمنية ذات مقياس زمني بنصف سنة . |
| HalfYearHh | `127` | الأمثلة هي H1 ، H2 |
| HalfYearHhYyy | `126` | الأمثلة هي H1 '10 ، H2 '10 |
| HalfYearHhhHalf | `123` | الأمثلة هي الشوط الأول ، النصف الثاني ، النصف الثاني |
| HalfYearHHyy | `129` | الأمثلة هي 1H10 ، 2H10 |
| HalfYearHlfH | `125` | الأمثلة هي نصف 1 ، نصف 2 |
| HalfYearHlfHYyyy | `124` | من الأمثلة النصف 1 ، 2010 ؛ نصف 2، 2010 |
| HalfYearFromEndH | `135` | الأمثلة هي 2 ، 1 ، -1 ، -2. نصف سنة من تاريخ انتهاء المشروع. |
| HalfYearFromEndHalfH | `133` | الأمثلة هي نصف 2 ، نصف 1 ، نصف -1 ، نصف -2 |
| HalfYearFromEndHh | `134` | الأمثلة هي H2 ، H1 ، H-1 ، H-2 |
| HalfYearFromStartH | `132` | الأمثلة هي -2 ، -1 ، 1 ، 2. نصف عام من تاريخ بدء المشروع. |
| HalfYearFromStartHalfH | `130` | الأمثلة هي نصف -2 ، نصف -1 ، نصف 1 ، نصف 2 |
| HalfYearFromStartHh | `131` | الأمثلة هي H-2 ، H-1 ، H1 ، H2 |
| HourDddMmmDdHhAm | `28` | الأمثلة هي الأربعاء 18 مارس ، 8 صباحًا ؛ الأربعاء 18 آذار (مارس) ، الساعة 9 صباحًا. يتطلب أن تكون الوحدة الزمنية ساعات مقياس الوقت. |
| HourHh | `32` | الأمثلة هي 8 ، 9 ، 10 ، 11 |
| HourHhMmAm | `30` | الأمثلة هي 8:00 صباحًا ، 9:00 صباحًا |
| HourHhAm | `31` | الأمثلة هي 8 ص ، 9 ص_ د |
| HourMmDdHhAm | `120` | الأمثلة هي 3/18 8 صباحًا ، 3/18 9 صباحًا |
| HourMmmDdHhAm | `29` | الأمثلة هي 18 مارس ، 8 صباحًا ؛ 18 آذار (مارس) 9 صباحًا |
| HourFromEndHh | `77` | الأمثلة هي 3 ، 2 ، 1 ، -1 ، -2 ساعة من نهاية المشروع. |
| HourFromEndHhh | `76` | الأمثلة هي H3 ، H2 ، H1 ، H-1 ، H-2 |
| HourFromEndHourHh | `39` | الأمثلة هي الساعة 3 ، الساعة 2 ، الساعة 1 ، الساعة -1 ، الساعة -2 |
| HourFromStartHh | `79` | الأمثلة هي -2 ، -1 ، 1 ، 2 ، 3 ساعات من بداية المشروع. |
| HourFromStartHhh | `78` | الأمثلة هي H-2 ، H-1 ، H1 ، H2 ، H3 |
| HourFromStartHourHh | `38` | الأمثلة هي الساعة -2 ، الساعة -1 ، الساعة 1 ، الساعة 2 ، الساعة 3 |
| MinuteHhMmAm | `33` | الأمثلة هي 8:00 صباحًا ، 8:01 صباحًا ، 8:02 صباحًا. يتطلب أن تكون الوحدة الزمنية دقيقة بمقياس الوقت. |
| MinuteMm | `34` | الأمثلة هي 0 ، 1 ، 2 ، ... ، 59 دقيقة |
| MinuteFromEndMinuteMm | `37` | الأمثلة هي الدقيقة 181 ، الدقيقة 180 ، ... ، الدقيقة 1 ، الدقيقة -1 من نهاية المشروع . |
| MinuteFromEndMm | `81` | الأمثلة هي 181 ، 180 ، ... ، 1 ، -1 |
| MinuteFromEndMmm | `80` | الأمثلة هي M181 ، M180 ، ... ، M1 ، M-1 |
| MinuteFromStartMinuteMm | `36` | الأمثلة هي الدقيقة -2 ، الدقيقة -1 ، الدقيقة 1 ، ... الدقيقة 180 من بداية المشروع . |
| MinuteFromStartMm | `83` | الأمثلة هي -2 ، -1 ، 1 ، ... ، 180 |
| MinuteFromStartMmm | `82` | الأمثلة هي M-2 ، M-1 ، M1 ، ... ، M180 |
| MonthM | `11` | الأمثلة هي M ، A ، M ، J ، J. تتطلب أن تكون الوحدة الزمنية هي TimescaleMonths . |
| MonthMm | `57` | الأمثلة هي 11 ، 12 ، 1 ، 2 |
| MonthMmYy | `86` | الأمثلة هي 3/10 ، 4/10 ، 5 / 10 |
| MonthMmYyy | `85` | الأمثلة هي 3 '10 ، 4 '10 ، 5 '10 |
| MonthMmm | `10` | الأمثلة هي مارس وأبريل ومايو |
| MonthMmmYyy | `8` | من الأمثلة على ذلك مارس '10 ، أبريل '10 ، مايو '10 |
| MonthMmmm | `9` | من الأمثلة مارس وأبريل ومايو |
| MonthMmmmYyyy | `7` | من الأمثلة مارس 2010 ، أبريل 2010 ، مايو 2010 |
| MonthFromEndMm | `59` | الأمثلة هي 2 ، 1 ، -1 ، -2 أشهر من نهاية المشروع. |
| MonthFromEndMmm | `58` | الأمثلة هي M2 ، M1 ، M-1 ، M-2 |
| MonthFromEndMonthMm | `45` | الأمثلة هي الشهر 2 ، الشهر 1 ، الشهر -1 ، الشهر -2 |
| MonthFromStartMm | `61` | الأمثلة هي -2 ، -2 ، 1 ، شهرين من بداية المشروع. |
| MonthFromStartMmm | `60` | الأمثلة هي M-2 و M-1 و M1 و M2 |
| MonthFromStartMonthMm | `44` | الأمثلة هي شهر -2 ، شهر -1 ، شهر 1 ، شهر 2 |
| QuarterQ | `62` | الأمثلة هي 3 ، 4 ، 1. تتطلب أن تكون وحدة الوقت على مقياس الوقت. |
| QuarterQq | `6` | الأمثلة هي Q3 ، Q4 ، Q1 |
| QuarterQqYyy | `4` | الأمثلة هي Q3 '10 ، Q4 '10 ، Q1 '11 |
| QuarterQqqQuarter | `2` | الأمثلة هي الربع الثالث ، والربع الأول |
| QuarterQQyy | `51` | الأمثلة هي 3Q10 ، 4Q10 ، 1Q11 |
| QuarterQtrQ | `5` | الأمثلة هي Qtr3 ، Qtr4 ، Qtr1 |
| QuarterQtrQYyyy | `3` | من الأمثلة Qtr3 ، 2010 ؛ الربع الرابع ، 2010 ؛ الربع الأول ، 2011 |
| QuarterFromEndQ | `64` | الأمثلة هي 5 ، 4 ، 3 ، 2 ، 1 ، -1 ربع من نهاية المشروع . |
| QuarterFromEndQq | `63` | الأمثلة هي Q5 ، Q4 ، Q3 ، Q2 ، Q1 ، Q-1 |
| QuarterFromEndQuarterQ | `47` | الأمثلة هي الربع الخامس ، والربع الرابع ، والربع الثالث ، والربع الثاني ، والربع الأول ، والربع -1 |
| QuarterFromStartQ | `66` | الأمثلة هي -5 ، -4 ، -3 ، -2 ، -1 ، 1 ربع من بداية المشروع . |
| QuarterFromStartQq | `65` | الأمثلة هي Q-5 و Q-4 و Q-3 و Q-2 و Q-1 و Q1 |
| QuarterFromStartQuarterQ | `46` | الأمثلة هي ربع -5 ، وربع -4 ، وربع -3 ، وربع -2 ، وربع -1 ، وربع 1 |
| ThirdsOfMonthsDd | `136` | الأمثلة هي 1 ، 11 ، 21 ، 1. تتطلب أن تكون الوحدة الزمنية مقياس الوقت للثالث من الأشهر . |
| ThirdsOfMonthsDdd | `137` | الأمثلة هي B ، M ، E ، B |
| ThirdsOfMonthsDddd | `138` | الأمثلة هي البداية ، والمتوسط ، والنهاية ، والبداية |
| ThirdsOfMonthsMmDd | `139` | المثال 3 / 1. |
| ThirdsOfMonthsMmDdYy | `145` | المثال هو 3/1 / 10. |
| ThirdsOfMonthsMmDdd | `140` | الأمثلة هي 3 / B ، 3 / M ، 3 / E ، 4 / B |
| ThirdsOfMonthsMmDddYy | `146` | المثال هو 3 / B / 10. |
| ThirdsOfMonthsMmmDd | `142` | الأمثلة هي 1 مارس ، 11 مارس ، 21 مارس ، 1 أبريل 1 |
| ThirdsOfMonthsMmmDdYy | `147` | من الأمثلة 1 مارس ، '10 ؛ 11 آذار (مارس) 2010 ؛ 21 آذار (مارس) 2010 ؛ 1 أبريل ، 10 |
| ThirdsOfMonthsMmmDdd | `143` | الأمثلة هي Mar B و Mar M و Mar E و April B |
| ThirdsOfMonthsMmmDddYy | `148` | من الأمثلة Mar B، '10؛ مار م ، 10 ؛ مار إي ، 10 ؛ أبريل ب '10 |
| ThirdsOfMonthsMmmmDd | `144` | من الأمثلة 1 آذار (مارس) ، 11 آذار (مارس) ، 21 آذار (مارس) ، 1 نيسان (أبريل) 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | من الأمثلة 1 آذار (مارس) 2010 ؛ 11 مارس 2010 ؛ 21 مارس 2010 ؛ 1 أبريل 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | الأمثلة هي بداية آذار (مارس) ، منتصف آذار (مارس) ، نهاية آذار (مارس) ، بداية نيسان (أبريل ) |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | من الأمثلة على ذلك بداية شهر آذار (مارس) 2010 ؛ منتصف مارس 2010 ؛ نهاية مارس 2010 ؛ بداية نيسان (أبريل) 2010 |
| WeekDddDd | `88` | من الأمثلة الأحد 21 ، الأحد 28 ، الأحد 4. يتطلب أن تكون الوحدة الزمنية هي أسابيع مقياس الوقت . |
| WeekDddMDd | `97` | الأمثلة هي Sun M 21 ، Sun M 28 ، Sun A 4 |
| WeekDddMmDd | `90` | الأمثلة هي الأحد 3/21 ، الأحد 3/28 ، الأحد 4/4 |
| WeekDddMmDdYy | `100` | الأمثلة هي الأحد 3/21/10 ، الأحد 3/28/10 ، الأحد 4/4/10 |
| WeekDddMmmDd | `93` | من الأمثلة الأحد 21 مارس ، الأحد 28 مارس ، الأحد 4 أبريل |
| WeekDddMmmDdYyy | `101` | من الأمثلة الأحد 21 مارس ، '10 ؛ الأحد 28 آذار (مارس) 2010 ؛ الأحد 4 إبريل ، '10 |
| WeekDddMmmmDd | `96` | الأمثلة الأحد 21 مارس ، الأحد 28 مارس ، الأحد أبريل 4 |
| WeekDddMmmmDdYyy | `102` | من الأمثلة الأحد 21 مارس ، '10 ؛ الأحد 28 مارس ، 2010 ؛ الأحد 4 أبريل '10 |
| WeekDddWw | `103` | من الأمثلة الأحد 12 ، الأحد 13 ، الأحد 14 |
| WeekDdiMDd | `98` | الأمثلة هي Su M 21 ، Su M 28 ، Su A 4 |
| WeekDdiMmDd | `91` | الأمثلة هي Su 3/21. سو 3/28 ، سو 4 / 4 |
| WeekDdiMmmDd | `94` | الأمثلة هي Su Mar 21 ، Su Mar 28 ، Su أبريل 4 |
| WeekDiMDd | `99` | الأمثلة هي SM 21 ، SM 28 ، SA 4 |
| WeekDiMmDd | `92` | الأمثلة هي S 3/21 ، S 3/28 ، S 4 / 4 |
| WeekDiMmmDd | `95` | الأمثلة هي S Mar 21 ، S Mar 28 ، S أبريل 4 |
| WeekMDd | `89` | الأمثلة هي M21 ، M28 ، A 4 |
| WeekMmDd | `17` | الأمثلة هي 3/21 ، 3/28 ، 4 / 4 |
| WeekMmDdYy | `16` | المثال هو "3/21/10" . |
| WeekMmmDd | `15` | الأمثلة هي 21 مارس ، 28 مارس ، 4 أبريل |
| WeekMmmDdYyy | `13` | من الأمثلة 21 آذار (مارس) ، '10 ؛ 28 آذار (مارس) 2010 ؛ 4 نيسان (أبريل) '10 |
| WeekMmmmDd | `14` | من الأمثلة 21 مارس ، 28 مارس ، 4 أبريل |
| WeekMmmmDdYyyy | `12` | من الأمثلة 21 آذار (مارس) 2010 ؛ 28 مارس 2010 ؛ 4 أبريل 2010 |
| WeekDayOfMonthDd | `87` | الأمثلة هي 21 ، 28 ، 4 |
| WeekFromEndWeekWw | `43` | من الأمثلة الأسبوع 2 ، الأسبوع 1 ، الأسبوع -1 من نهاية المشروع. |
| WeekFromEndWw | `68` | الأمثلة هي 2 ، 1 ، -1 |
| WeekFromEndWww | `67` | الأمثلة هي W2 و W1 و W-1 |
| WeekFromStartWeekWw | `42` | الأمثلة هي الأسبوع -1 ، الأسبوع 1 ، الأسبوع 2 من بداية المشروع . |
| WeekFromStartWw | `70` | الأمثلة هي -1 ، 1 ، 2 |
| WeekFromStartWww | `69` | الأمثلة هي W-1 و W1 و W2 |
| WeekNumberDdWw | `104` | الأمثلة هي 12 1 و 13 و 1 14 (اليوم 1 من الأسبوع 12 واليوم 1 من الأسبوع 13 وهكذا) |
| WeekNumberWw | `50` | الأمثلة هي 12 ، 13 ، 14 |
| YearYy | `75` | الأمثلة هي 10 ، 11 ، 12. تتطلب أن تكون الوحدة الزمنية هي السنة الزمنية . |
| YearYyy | `1` | الأمثلة هي "10 ،" 11 ، "12 |
| YearYyyy | `0` | الأمثلة 2010 ، 2011 ، 2012 |
| YearFromEndYearYy | `49` | الأمثلة هي السنة 2 ، السنة 1 ، السنة -1 من نهاية المشروع. |
| YearFromEndYy | `72` | الأمثلة هي 2 ، 1 ، -1 |
| YearFromEndYyy | `71` | الأمثلة هي Y2 و Y1 و Y-1 |
| YearFromStartYearYy | `48` | الأمثلة هي السنة -1 ، السنة 1 ، السنة 2 من بداية المشروع . |
| YearFromStartYy | `74` | الأمثلة هي -1 ، 1 ، 2 |
| YearFromStartYyy | `73` | الأمثلة هي Y-1 و Y1 و Y2 |

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks.Visualization](../../aspose.tasks.visualization)
* المجسم [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->