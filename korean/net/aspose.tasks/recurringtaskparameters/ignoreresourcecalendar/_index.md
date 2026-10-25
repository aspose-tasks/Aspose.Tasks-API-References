---
title: "RecurringTaskParameters.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RecurringTaskParameters 속성. 리소스가 작업 가능할 때가 아니더라도 반복 작업을 예약할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

리소스가 사용 가능하지 않을 때에도 반복 작업을 예약할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool IgnoreResourceCalendar { get; set; }
```

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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


