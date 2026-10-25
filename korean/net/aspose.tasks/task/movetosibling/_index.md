---
title: "Task.MoveToSibling"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 현재 작업을 지정된 작업 앞의 동일한 개요 수준으로 이동합니다. ParentProject.CalculationMode가 None인 경우 사용자는 이 메서드 사용 후 Project.Recalculate를 호출해야 합니다. 이 메서드는 모든 프로젝트 작업의 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드와 같은 종속 필드를 계산합니다. ParentProject.CalculationMode가 Manual인 경우 메서드는 작업 ID와 개요 수준, 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우 메서드는 모든 프로젝트 작업을 자동으로 재조정하고 시작/완료 날짜를 설정하며, 조기/지연 날짜를 설정하고, 여유시간, 작업 및 비용 필드를 계산하며, ID와 개요 수준을 재계산합니다."
type: docs
weight: 1370
url: /ko/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

현재 작업을 동일한 Outline Level에서 지정된 작업 앞에 이동합니다. ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후에 Project.Recalculate()를 호출해야 합니다(이 메서드는 모든 프로젝트 작업(시작/완료 날짜, 조기/지연 날짜 설정)을 재조정하고, 여유시간, 작업 및 비용 필드, Outline Level과 같은 종속 필드를 계산합니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 Id, Outline Level 및 Outline 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정합니다(시작/완료 날짜, 조기/지연 날짜 설정, 여유시간, 작업 및 비용 필드 계산, Id 및 Outline Level 재계산).

```csharp
public void MoveToSibling(Task beforeTask)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| beforeTask | 작업 | 현재 작업이 삽입될 앞의 Task. |

## 예제

동일한 상위 작업 아래에서 작업을 이동하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// ID가 5인 작업을 ID가 3인 작업 앞으로 이동합니다.
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// 또는
// 작업을 컬렉션의 끝으로 이동합니다.
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

현재 작업을 동일한 Outline Level에서 지정된 Id를 가진 작업 앞에 이동합니다. ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후에 Project.Recalculate()를 호출해야 합니다(이 메서드는 모든 프로젝트 작업(시작/완료 날짜, 조기/지연 날짜 설정)을 재조정하고, 여유시간, 작업 및 비용 필드, Outline Level과 같은 종속 필드를 계산합니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 Id, Outline Level 및 Outline 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정합니다(시작/완료 날짜, 조기/지연 날짜 설정, 여유시간, 작업 및 비용 필드 계산, Id 및 Outline Level 재계산).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| beforeTaskId | Int32 | 현재 작업이 삽입될 앞의 작업의 Id ([`Id`](../../tsk/id/)). |

## 예제

작업의 Id를 사용하여 동일한 상위 작업 아래에서 작업을 이동하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// ID가 5인 작업을 ID가 3인 작업 앞으로 이동합니다.
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// 또는
// 작업을 컬렉션의 끝으로 이동합니다.
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


