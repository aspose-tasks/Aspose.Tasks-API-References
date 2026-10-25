---
title: "열거형 Month"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Month 열거형. 월을 지정합니다."
type: docs
weight: 1040
url: /ko/net/aspose.tasks/month/
---
## Month enumeration

월을 지정합니다.

```csharp
public enum Month
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 원본 프로젝트 파일에 값이 정의되지 않았음을 나타냅니다. |
| January | `0` | 1월을 나타냅니다. |
| February | `1` | 2월을 나타냅니다. |
| March | `2` | 3월을 나타냅니다. |
| April | `3` | 4월을 나타냅니다. |
| May | `4` | 5월을 나타냅니다. |
| June | `5` | 6월을 나타냅니다. |
| July | `6` | 7월을 나타냅니다. |
| August | `7` | 8월을 나타냅니다. |
| September | `8` | 9월을 나타냅니다. |
| October | `9` | 10월을 나타냅니다. |
| November | `10` | 11월을 나타냅니다. |
| December | `11` | 12월을 나타냅니다. |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

새로운 반복 작업을 생성하면서 연도 일 반복을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


