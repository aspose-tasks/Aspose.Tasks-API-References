---
title: DateLabel
second_title: .NET API 참조용 Aspose.Tasks
description: 시간 척도에서 날짜 및 시간 레이블의 표시 형식을 지정합니다.
type: docs
weight: 2650
url: /ko/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

시간 척도에서 날짜 및 시간 레이블의 표시 형식을 지정합니다.

```csharp
public enum DateLabel
```

### 가치

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `35` | 날짜가 표시되지 않습니다. |
| DayDdd | `19` | 예는 Mon, Tue입니다. |
| DayDddDd | `105` | 예: Mon 30, Tue 1 |
| DayDddMDd | `112` | 예: Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | 예: Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | 예: Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | 예는 9월 30일 월요일, 10월 1일 화요일 입니다. |
| DayDddMmmDdYyy | `22` | 예는 Mon Sep 30 '02, Tue Oct 1 '02 입니다. |
| DayDddMmmmDd | `111` | 예는 9월 30일 월요일, 10월 1일 화요일 입니다. |
| DayDddd | `18` | 예는 화요일, 수요일입니다. |
| DayDdi | `119` | 예는 Mo, Tu 입니다. |
| DayDdiDd | `106` | 예는 Mo 30, Tu 1 입니다. |
| DayDdiMDd | `113` | 예는 Mo S 30, Tu O 1 입니다. |
| DayDdiMmDd | `109` | 예는 Mo 9/30, Tu 10/1 입니다. |
| DayDi | `20` | 예는 M, T 입니다. |
| DayDiDdSpace | `107` | 예는 M 30, T 1 입니다. |
| DayDiMDd | `114` | 예는 MS 30, TO 1 입니다. |
| DayDiMmDd | `110` | 예: M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | 예는 M30, T1 입니다. |
| DayMDd | `115` | 예는 S 30, O 1 입니다. |
| DayMmDd | `27` | 예는 9/30, 10/1 입니다. |
| DayMmDdYy | `26` | 예는 9/30/02, 10/1/02 입니다. |
| DayMmmDd | `25` | 예: 9월 30일, 10월 1일 |
| DayMmmDdYyy | `24` | 예는 '02년 9월 30일, '02 10월 10일입니다. |
| DayFromEndDayDd | `41` | 예는 프로젝트 끝에서 Day 2, Day 1, Day -1, Day -2입니다. |
| DayFromEndDd | `54` | 예는 2, 1, -1, -2 입니다. |
| DayFromEndDdd | `53` | 예는 D2, D1, D-1, D-2 입니다. |
| DayFromStartDayDd | `40` | 예는 프로젝트 시작부터 Day -2, Day -1, Day 1, Day 2입니다. |
| DayFromStartDd | `56` | 예는 -2, -1, 1, 2 입니다. |
| DayFromStartDdd | `55` | 예는 D-2, D-1, D1, D2 입니다. |
| DayOfMonthDd | `21` | 예는 30, 1 |
| DayOfYearDd | `118` | 예는 77, 78 입니다. |
| DayOfYearDdYyy | `116` | 예는 77 '10, 78 '10 입니다. |
| DayOfYearDdYyyy | `117` | 예는 77 2010, 78 2010 입니다. |
| DayDdMmYyyy | `256` | 예는 19/07/2016. |
| HalfYearH | `128` | 예는 1, 2입니다. 시간 단위는 TimescaleHalfYears. 여야 합니다. |
| HalfYearHh | `127` | 예는 H1, H2 입니다. |
| HalfYearHhYyy | `126` | 예는 H1 '10, H2 '10 입니다. |
| HalfYearHhhHalf | `123` | 예는 1st Half, 2d Half 입니다. |
| HalfYearHHyy | `129` | 예는 1H10, 2H10 입니다. |
| HalfYearHlfH | `125` | 예는 Half 1, Half 2 입니다. |
| HalfYearHlfHYyyy | `124` | 예는 Half 1, 2010; 하프 2, 2010 |
| HalfYearFromEndH | `135` | 예는 2, 1, -1, -2입니다. 프로젝트 종료일로부터 반년. |
| HalfYearFromEndHalfH | `133` | 예는 Half 2, Half 1, Half -1, Half -2 입니다. |
| HalfYearFromEndHh | `134` | 예는 H2, H1, H-1, H-2 입니다. |
| HalfYearFromStartH | `132` | 예는 -2, -1, 1, 2입니다. 프로젝트 시작일로부터 반년. |
| HalfYearFromStartHalfH | `130` | 예는 Half -2, Half -1, Half 1, Half 2 입니다. |
| HalfYearFromStartHh | `131` | 예는 H-2, H-1, H1, H2 입니다. |
| HourDddMmmDdHhAm | `28` | 예는 3월 18일 수요일 오전 8시입니다. 3월 18일 수요일 오전 9시. 시간 단위는 TimescaleHours. 여야 합니다. |
| HourHh | `32` | 예는 8, 9, 10, 11 입니다. |
| HourHhMmAm | `30` | 예: 오전 8시, 오전 9시 |
| HourHhAm | `31` | 예: 오전 8시, 오전 9시 |
| HourMmDdHhAm | `120` | 예는 3/18 오전 8시, 3/18 오전 9시 입니다. |
| HourMmmDdHhAm | `29` | 예는 3월 18일 오전 8시입니다. 3월 18일 오전 9시 |
| HourFromEndHh | `77` | 예는 프로젝트 종료로부터 3, 2, 1, -1, -2시간입니다. |
| HourFromEndHhh | `76` | 예는 H3, H2, H1, H-1, H-2 입니다. |
| HourFromEndHourHh | `39` | 예는 시간 3, 시간 2, 시간 1, 시간 -1, 시간 -2 입니다. |
| HourFromStartHh | `79` | 예는 프로젝트 시작부터 -2, -1, 1, 2, 3시간입니다. |
| HourFromStartHhh | `78` | 예는 H-2, H-1, H1, H2, H3 입니다. |
| HourFromStartHourHh | `38` | 예: 시 -2, 시 -1, 시 1, 시 2, 시 3 |
| MinuteHhMmAm | `33` | 예는 오전 8:00, 오전 8:01, 오전 8:02입니다. 시간 단위는 TimescaleMinutes. 여야 합니다. |
| MinuteMm | `34` | 예는 0, 1, 2, ..., 59분입니다. |
| MinuteFromEndMinuteMm | `37` | 예는 프로젝트 끝에서 181분, 180분, ..., 1분, -1분입니다. |
| MinuteFromEndMm | `81` | 예는 181, 180, ..., 1, -1 입니다. |
| MinuteFromEndMmm | `80` | 예는 M181, M180, ..., M1, M-1 입니다. |
| MinuteFromStartMinuteMm | `36` | 예: Minute -2, Minute -1, Minute 1, ... Minute 180 from the project start. |
| MinuteFromStartMm | `83` | 예는 -2, -1, 1, ..., 180 입니다. |
| MinuteFromStartMmm | `82` | 예는 M-2, M-1, M1, ..., M180 입니다. |
| MonthM | `11` | 예는 M, A, M, J, J입니다. 시간 단위는 TimescaleMonths여야 합니다. |
| MonthMm | `57` | 예는 11, 12, 1, 2 입니다. |
| MonthMmYy | `86` | 예는 3/10, 4/10, 5/10 입니다. |
| MonthMmYyy | `85` | 예는 3 '10, 4 '10, 5 '10 입니다. |
| MonthMmm | `10` | 예는 Mar, Apr, May 입니다. |
| MonthMmmYyy | `8` | 예는 '10년 3월, '10년 4월, '10년 5월 입니다. |
| MonthMmmm | `9` | 예는 3월, 4월, 5월 입니다. |
| MonthMmmmYyyy | `7` | 예는 2010년 3월, 2010년 4월, 2010년 5월 입니다. |
| MonthFromEndMm | `59` | 예는 프로젝트 종료 후 2, 1, -1, -2개월입니다. |
| MonthFromEndMmm | `58` | 예는 M2, M1, M-1, M-2 입니다. |
| MonthFromEndMonthMm | `45` | 예는 월 2, 월 1, 월 -1, 월 -2 입니다. |
| MonthFromStartMm | `61` | 예는 프로젝트 시작으로부터 -2, -2, 1, 2개월입니다. |
| MonthFromStartMmm | `60` | 예는 M-2, M-1, M1, M2 입니다. |
| MonthFromStartMonthMm | `44` | 예: 월 -2, 월 -1, 월 1, 월 2 |
| QuarterQ | `62` | 예는 3, 4, 1입니다. 시간 단위는 TimescaleQuarters. 여야 합니다. |
| QuarterQq | `6` | 예는 Q3, Q4, Q1 입니다. |
| QuarterQqYyy | `4` | 예는 Q3 '10, Q4 '10, Q1 '11 입니다. |
| QuarterQqqQuarter | `2` | 예는 3분기, 1분기 입니다. |
| QuarterQQyy | `51` | 예는 3Q10, 4Q10, 1Q11 입니다. |
| QuarterQtrQ | `5` | 예는 Qtr3, Qtr4, Qtr1 입니다. |
| QuarterQtrQYyyy | `3` | 예는 Qtr3, 2010입니다. 2010년 4분기; 2011년 1분기 |
| QuarterFromEndQ | `64` | 예는 프로젝트 끝에서 5, 4, 3, 2, 1, -1 분기입니다. |
| QuarterFromEndQq | `63` | 예는 Q5, Q4, Q3, Q2, Q1, Q-1 입니다. |
| QuarterFromEndQuarterQ | `47` | 예: 분기 5, 분기 4, 분기 3, 분기 2, 분기 1, 분기 -1 |
| QuarterFromStartQ | `66` | 예는 프로젝트 시작부터 -5, -4, -3, -2, -1, 1분기입니다. |
| QuarterFromStartQq | `65` | 예는 Q-5, Q-4, Q-3, Q-2, Q-1, Q1 입니다. |
| QuarterFromStartQuarterQ | `46` | 예: 분기 -5, 분기 -4, 분기 -3, 분기 -2, 분기 -1, 분기 1 |
| ThirdsOfMonthsDd | `136` | 예는 1, 11, 21, 1입니다. 시간 단위는 TimescaleThirdsOfMonths. 여야 합니다. |
| ThirdsOfMonthsDdd | `137` | 예는 B, M, E, B 입니다. |
| ThirdsOfMonthsDddd | `138` | 예는 시작, 중간, 끝, Beginning 입니다. |
| ThirdsOfMonthsMmDd | `139` | 예는 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | 예는 3/1/10. 입니다. |
| ThirdsOfMonthsMmDdd | `140` | 예는 3/B, 3/M, 3/E, 4/B 입니다. |
| ThirdsOfMonthsMmDddYy | `146` | 예는 3/B/10. 입니다. |
| ThirdsOfMonthsMmmDd | `142` | 예는 3월 1일, 3월 11일, 3월 21일, 4월 1일 입니다. |
| ThirdsOfMonthsMmmDdYy | `147` | 예는 '10년 3월 1일; 2010년 3월 11일; 2010년 3월 21일; 10 4월 1일 |
| ThirdsOfMonthsMmmDdd | `143` | 예는 Mar B, Mar M, Mar E, Apr B 입니다. |
| ThirdsOfMonthsMmmDddYy | `148` | 예는 Mar B, '10; 3월 M, '10; 2010년 3월; 4월 B '10 |
| ThirdsOfMonthsMmmmDd | `144` | 예는 3월 1일, 3월 11일, 3월 21일, 4월 1일 입니다. |
| ThirdsOfMonthsMmmmDdYyyy | `149` | 예는 2010년 3월 1일입니다. 2010년 3월 11일; 2010년 3월 21일; 2010년 4월 1일 |
| ThirdsOfMonthsMmmmDddd | `141` | 예는 3월 시작, 3월 중간, 3월 말, 4월 시작 입니다. |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | 예는 2010년 3월 초; 2010년 3월 중순; 2010년 3월 말; 4월 초, 2010 |
| WeekDddDd | `88` | 예는 Sun 21, Sun 28, Sun 4입니다. 시간 단위는 TimescaleWeeks여야 합니다. |
| WeekDddMDd | `97` | 예는 Sun M 21, Sun M 28, Sun A 4 입니다. |
| WeekDddMmDd | `90` | 예는 Sun 3/21, Sun 3/28, Sun 4/4 입니다. |
| WeekDddMmDdYy | `100` | 예는 Sun 3/21/10, Sun 3/28/10, Sun 4/4/10 입니다. |
| WeekDddMmmDd | `93` | 예는 3월 21일 일요일, 3월 28일 일요일, 4월 4일 일요일 입니다. |
| WeekDddMmmDdYyy | `101` | 예는 Sun Mar 21, '10; 2010년 3월 28일 일요일; 4월 4일, '10 |
| WeekDddMmmmDd | `96` | 예는 3월 21일 일요일, 3월 28일 일요일, 4월 4일 일요일 입니다. |
| WeekDddMmmmDdYyy | `102` | 예는 '10년 3월 21일 일요일입니다. 10년 3월 28일 일요일; 4월 4일 일요일 '10 |
| WeekDddWw | `103` | 예는 Sun 12, Sun 13, Sun 14 입니다. |
| WeekDdiMDd | `98` | 예는 Su M 21, Su M 28, Su A 4 입니다. |
| WeekDdiMmDd | `91` | 예는 Su 3/21입니다. 수 3/28, 수 4/4 |
| WeekDdiMmmDd | `94` | 예는 Su Mar 21, Su Mar 28, Su Apr 4 입니다. |
| WeekDiMDd | `99` | 예는 SM 21, SM 28, SA 4 입니다. |
| WeekDiMmDd | `92` | 예는 S 3/21, S 3/28, S 4/4 입니다. |
| WeekDiMmmDd | `95` | 예: S 3월 21일, S 3월 28일, S 4월 4일 |
| WeekMDd | `89` | 예는 M21, M28, A 4 입니다. |
| WeekMmDd | `17` | 예는 3/21, 3/28, 4/4 입니다. |
| WeekMmDdYy | `16` | 예는 '3/21/10'입니다. |
| WeekMmmDd | `15` | 예: 3월 21일, 3월 28일, 4월 4일 |
| WeekMmmDdYyy | `13` | 예는 '10년 3월 21일; 2010년 3월 28일; 4월 4일, '10 |
| WeekMmmmDd | `14` | 예는 3월 21일, 3월 28일, 4월 4일 입니다. |
| WeekMmmmDdYyyy | `12` | 예는 2010년 3월 21일입니다. 2010년 3월 28일; 2010년 4월 4일 |
| WeekDayOfMonthDd | `87` | 예는 21, 28, 4 입니다. |
| WeekFromEndWeekWw | `43` | 예는 프로젝트 끝에서 2주차, 1주차, -1주차입니다. |
| WeekFromEndWw | `68` | 예는 2, 1, -1 입니다. |
| WeekFromEndWww | `67` | 예는 W2, W1, W-1 입니다. |
| WeekFromStartWeekWw | `42` | 예는 프로젝트 시작부터 -1주차, 1주차, 2주차입니다. |
| WeekFromStartWw | `70` | 예는 -1, 1, 2 입니다. |
| WeekFromStartWww | `69` | 예는 W-1, W1, W2 입니다. |
| WeekNumberDdWw | `104` | 예는 1 12, 1 13, 1 14(12주 1일, 13주 1일 등) 입니다. |
| WeekNumberWw | `50` | 예는 12, 13, 14 입니다. |
| YearYy | `75` | 예는 10, 11, 12입니다. 시간 단위는 TimescaleYears. 여야 합니다. |
| YearYyy | `1` | 예는 '10, '11, '12 입니다. |
| YearYyyy | `0` | 예는 2010, 2011, 2012 입니다. |
| YearFromEndYearYy | `49` | 예는 프로젝트 끝에서 2년차, 1년차, -1년차입니다. |
| YearFromEndYy | `72` | 예는 2, 1, -1 입니다. |
| YearFromEndYyy | `71` | 예는 Y2, Y1, Y-1 입니다. |
| YearFromStartYearYy | `48` | 예는 프로젝트 시작부터 Year -1, Year 1, Year 2입니다. |
| YearFromStartYy | `74` | 예는 -1, 1, 2 입니다. |
| YearFromStartYyy | `73` | 예는 Y-1, Y1, Y2 입니다. |

### 또한보십시오

* 네임스페이스 [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
