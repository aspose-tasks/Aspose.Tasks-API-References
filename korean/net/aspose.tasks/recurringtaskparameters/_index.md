---
title: "클래스 RecurringTaskParameters"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RecurringTaskParameters 클래스. 프로젝트에서 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다."
type: docs
weight: 1730
url: /ko/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

프로젝트에서 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다.

```csharp
public class RecurringTaskParameters
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | `RecurringTaskParameters` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | 반복 작업 한 번 발생에 대한 기간을 가져오거나 설정합니다. [`Duration`](./duration/) 클래스의 인스턴스입니다. |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | 리소스가 사용 가능하지 않을 때에도 반복 작업을 예약할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | 반복 작업의 반복 패턴을 가져오거나 설정합니다. [`RecurrencePattern`](./recurrencepattern/) 열거형의 값 중 하나일 수 있습니다. |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | 반복 작업의 이름을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | 반복 작업에 대한 캘린더를 설정합니다. 캘린더는 프로젝트 캘린더 컬렉션에서 선택됩니다. |

## 예제

반복 작업을 만드는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


