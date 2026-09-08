---
title: "클래스 TaskLink"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskLink 클래스. 선행 링크를 나타냅니다."
type: docs
weight: 2410
url: /ko/net/aspose.tasks/tasklink/
---
## TaskLink class

선행 작업 링크를 나타냅니다.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | 외부 선행 프로젝트를 가져오거나 설정합니다. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | 선행 작업이 다른 프로젝트의 일부인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | 지연 형식을 표현하는 포맷을 가져오거나 설정합니다. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | 분의 10분의 1 또는 백분율로 지연을 가져오거나 설정합니다. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | LagFormat에 따라 지연 지속 시간을 가져오거나 설정합니다. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | 링크 유형을 가져오거나 설정합니다. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | 선행 작업을 가져오거나 설정합니다. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | 후속 작업을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | `TaskLink` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | TaskLink의 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다. |

## 예제

프로젝트 작업 링크를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// 선행 작업 및 후속 작업의 이름을 표시합니다.
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


