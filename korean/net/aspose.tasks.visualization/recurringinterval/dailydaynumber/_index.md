---
title: "RecurringInterval.DailyDayNumber"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RecurringInterval 속성. 일별 날짜 번호를 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/recurringinterval/dailydaynumber/
---
## RecurringInterval.DailyDayNumber property

일일 날짜 번호를 가져오거나 설정합니다.

```csharp
public int DailyDayNumber { get; set; }
```

## 예제

진행 라인의 일일 반복 간격을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// 일일 패턴 날짜 번호를 설정합니다.
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// 일일 진행 라인에 대해 해당 날짜가 근무일인지 여부를 나타내는 값을 설정합니다.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### 또 보기

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


