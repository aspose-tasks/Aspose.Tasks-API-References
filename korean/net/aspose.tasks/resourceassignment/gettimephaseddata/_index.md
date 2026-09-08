---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 지정된 TimephasedDataType의 시작 및 종료 날짜 내에 TimephasedData 클래스 인스턴스를 포함하는 TimephasedDataCollection 클래스 인스턴스를 반환합니다."
type: docs
weight: 720
url: /ko/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

지정된 [`TimephasedDataType`](../../timephaseddatatype/)의 시작 및 종료 날짜 내에 [`TimephasedData`](../timephaseddata/) 클래스 인스턴스를 포함하는 [`TimephasedDataCollection`](../../timephaseddatacollection/) 클래스 인스턴스를 반환합니다.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 시간 단계 데이터의 시작 날짜입니다. |
| 끝 | DateTime | 시간 단계 데이터의 종료 날짜입니다. |
| timephasedType | TimephasedDataType | 시간 단계 데이터 유형 ([`TimephasedDataType`](../../timephaseddatatype/))입니다. |

### 반환 값

[`TimephasedData`](../../timephaseddata/) 클래스 인스턴스를 포함하는 목록을 반환합니다.

## 예제

날짜 범위 내에서 리소스 할당의 시간별 데이터를 생성하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// 프로젝트 속성을 설정합니다.
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// 리소스 할당을 생성합니다.
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Backloaded 컨투어를 설정하면 작업 기간이 6일에서 10일로 증가합니다.
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// 시간별 데이터를 가져옵니다.
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

주어진 AssignmentWork의 시작 및 종료 날짜 내에 [`TimephasedData`](../timephaseddata/) 클래스 인스턴스를 포함하는 [`TimephasedDataCollection`](../../timephaseddatacollection/) 객체를 반환합니다.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 시간 단계 데이터의 시작 날짜입니다. |
| 끝 | DateTime | 시간 단계 데이터의 종료 날짜입니다. |

### 반환 값

[`TimephasedData`](../../timephaseddata/) 클래스 인스턴스를 포함하는 목록을 반환합니다.

## 예제

날짜 범위 내에서 리소스 할당의 시간별 데이터를 생성하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// 프로젝트 속성을 설정합니다.
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// 리소스 할당을 생성합니다.
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Backloaded 컨투어를 설정하면 작업 기간이 6일에서 10일로 증가합니다.
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// 시간별 데이터를 가져옵니다.
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


