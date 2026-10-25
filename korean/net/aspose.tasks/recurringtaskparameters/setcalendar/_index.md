---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RecurringTaskParameters 메서드. 반복 작업에 대한 캘린더를 설정합니다. 캘린더는 프로젝트 캘린더 컬렉션에서 선택됩니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

반복 작업에 대한 캘린더를 설정합니다. 캘린더는 프로젝트 캘린더 컬렉션에서 선택됩니다.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | 캘린더 컬렉션이 있는 프로젝트입니다. |
| calendarName | 문자열 | 캘린더의 이름입니다. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


