---
title: "열거형 GroupOn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GroupOn 열거형. 그룹화 유형을 지정합니다."
type: docs
weight: 810
url: /ko/net/aspose.tasks/groupon/
---
## GroupOn enumeration

그룹화 유형을 지정합니다.

```csharp
public enum GroupOn
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| DateDay | `13` | 날짜를 기준으로 일별 그룹화합니다. |
| DateEachValue | `10` | 각 값에 대해 날짜별 그룹화합니다. |
| DateHour | `12` | 날짜를 시간별로 그룹화합니다. |
| DateMinute | `11` | 날짜를 분별로 그룹화합니다. |
| DateMonth | `16` | 날짜를 월별로 그룹화합니다. |
| DateQtr | `17` | 날짜를 분기별로 그룹화합니다. |
| DateThirdOfMonth | `15` | 날짜를 한 달의 3분의 1마다 그룹화합니다. |
| DateWeek | `14` | 날짜를 주별로 그룹화합니다. |
| DateYear | `18` | 날짜를 연도별로 그룹화합니다. |
| DurationDays | `23` | 기간을 일별로 그룹화합니다. |
| DurationEachValue | `20` | 각 값에 대해 기간을 그룹화합니다. |
| DurationHours | `22` | 기간을 시간별로 그룹화합니다. |
| DurationMinutes | `21` | 기간을 분별로 그룹화합니다. |
| DurationMonths | `25` | 기간을 월별로 그룹화합니다. |
| DurationWeeks | `24` | 기간을 주별로 그룹화합니다. |
| EachValue | `0` | 각 값별로 그룹화합니다. |
| Interval | `1` | 간격별로 그룹화합니다. |
| OutlineEachValue | `30` | 각 개요 값별로 그룹화합니다. |
| OutlineLevel | `31` | 개요 수준별로 그룹화합니다. |
| Pct110 | `45` | 10% 완료 증가 단위별로 그룹화합니다. |
| Pct125 | `44` | 25% 완료 증가 단위별로 그룹화합니다. |
| Pct150 | `43` | 50% 완료 증가 단위별로 그룹화합니다. |
| Pct199 | `42` | 99% 완료 기준으로 그룹화합니다. |
| PctEachValue | `40` | 각 값의 백분율별로 그룹화합니다. |
| PctInterval | `41` | 간격 백분율별로 그룹화합니다. |
| TextEachValue | `50` | 각 텍스트 값별로 그룹화합니다. |
| TextPrefix | `51` | 텍스트 접두사별로 그룹화합니다. |

## 예제

그룹 기준의 속성을 읽는 방법을 보여줍니다.

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

// 기준의 배경 패턴을 읽습니다
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


