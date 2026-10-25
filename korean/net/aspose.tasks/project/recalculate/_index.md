---
title: "Project.Recalculate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 모든 프로젝트 작업의 ID, 개요 수준, 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산합니다."
type: docs
weight: 1150
url: /ko/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜를 재조정하고, 조기/후기 날짜를 설정하며, 여유 시간, 작업 및 비용 필드를 계산합니다.

```csharp
public void Recalculate()
```

## 예제

프로젝트를 종료 날짜가 아니라 시작 날짜부터 다시 일정 잡는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// 이제 모든 작업 날짜(Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish)가 계산됩니다. 임계 경로를 얻으려면 여유 시간을 계산해야 합니다(별도의 스레드에서 호출할 수 있지만 모든 조기/지연 날짜 계산 후에만 가능합니다).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

옵션 검증을 포함하여 모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜를 재조정하고, 조기/후기 날짜를 설정하며, 여유 시간, 작업 및 비용 필드를 계산합니다.

```csharp
public void Recalculate(bool validate)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| validate | Boolean | true이면 재계산 검증이 수행됩니다. 검증되는 데이터: 현재는 작업 및 작업 링크 날짜 범위에 대한 기본 검증만 구현되어 있습니다. 작업의 날짜 범위(예: ActualStart - ActualFinish, EarlyStart - EarlyFinish 등)와 작업 링크 날짜는 시작 날짜가 종료 날짜보다 작거나 같은지 확인하는 기준에 따라 검사됩니다. 위에 설명된 조건 중 하나라도 실패하면 [`RecalculationValidationException`](../../recalculationvalidationexception/)이 발생합니다. |

## 예제

후 검증과 함께 프로젝트를 재계산하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // 후 검증과 함께 프로젝트를 재계산합니다
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


