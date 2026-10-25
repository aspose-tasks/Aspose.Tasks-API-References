---
title: "Task.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 지정된 시간 구분 데이터 유형의 주어진 시작 및 종료 날짜 내에 있는 TimephasedData 값을 포함하는 TimephasedDataCollection 객체를 반환합니다."
type: docs
weight: 1360
url: /ko/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

지정된 시간 구분 데이터 유형의 주어진 시작 및 종료 날짜 내에 있는 [`TimephasedData`](../timephaseddata/) 값을 포함하는 [`TimephasedDataCollection`](../../timephaseddatacollection/) 객체를 반환합니다.

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

지정된 시간 구분 데이터 유형의 주어진 시작 및 종료 날짜 내에 있는 [`TimephasedData`](../timephaseddata/) 값을 포함하는 [`TimephasedDataCollection`](../../timephaseddatacollection/) 객체입니다.

## 예제

작업의 시간 구분 데이터(특정 유형 포함)를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

주어진 시작 및 종료 날짜 내에 있는 [`TimephasedData`](../timephaseddata/) 값을 포함하는 [`TimephasedDataCollection`](../../timephaseddatacollection/) 객체를 반환합니다.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 시간 단계 데이터의 시작 날짜입니다. |
| 끝 | DateTime | 시간 단계 데이터의 종료 날짜입니다. |

### 반환 값

채워야 할 [`TimephasedData`](../../timephaseddata/) 목록입니다.

## 예제

작업의 timephased 데이터 (TaskWork 유형 포함)를 가져오는 방법을 보여줍니다.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


