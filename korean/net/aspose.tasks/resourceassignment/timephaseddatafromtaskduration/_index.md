---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 작업 기간 및 예정 시작 날짜를 기준으로 시간 구분 데이터 목록을 생성합니다."
type: docs
weight: 780
url: /ko/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

작업 기간 및 예정 시작 날짜를 기준으로 시간 구분 데이터 목록을 생성합니다.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 캘린더 | Calendar | 시간 구분 데이터를 생성할 캘린더. |

## 예제

작업에 분할을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 표준 캘린더 가져오기
var calendar = project.Get(Prj.Calendar);

// 프로젝트의 캘린더 설정을 지정합니다.
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// 루트 작업에 새 작업을 추가합니다.
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// 새 리소스 할당을 생성하고 시간 구분 데이터를 생성합니다.
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// 작업을 3부분으로 분할합니다.
// 분할에 사용할 SplitTask 메서드에 시작 날짜와 종료 날짜 인수를 제공합니다.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


