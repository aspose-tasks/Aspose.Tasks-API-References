---
title: "Resource.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 메서드. 지정된 TimephasedDataType의 시작 및 종료 날짜 내에 있는 TimephasedData 값을 포함하는 이 객체에 대한 TimephasedDataCollection 클래스의 인스턴스를 반환합니다."
type: docs
weight: 850
url: /ko/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

이 객체에 대해 지정된 [`TimephasedDataType`](../../timephaseddatatype/)의 시작 및 종료 날짜 내에 있는 [`TimephasedData`](../timephaseddata/) 값을 포함하는 [`TimephasedDataCollection`](../../timephaseddatacollection/) 클래스의 인스턴스를 반환합니다.

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

[`TimephasedData`](../timephaseddata/) 목록.

## 예제

작업/비용 리소스의 시간 단계 데이터를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// ID로 Resource를 가져옵니다.
var resource = project.Resources.GetByUid(1);

// ResourceWork의 시간 단계 데이터를 출력합니다.
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// ResourceCost의 시간 단계 데이터를 출력합니다.
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

이 객체에 대해 주어진 시작 및 종료 날짜 내에 있는 [`TimephasedData`](../timephaseddata/) 값을 포함하는 [`TimephasedDataCollection`](../../timephaseddatacollection/)을 반환합니다.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 시간 단계 데이터의 시작 날짜입니다. |
| 끝 | DateTime | 시간 단계 데이터의 종료 날짜입니다. |

### 반환 값

[`TimephasedData`](../../timephaseddata/) 목록.

## 예제

작업/비용 리소스의 시간 단계 데이터를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// ID로 Resource를 가져옵니다.
var resource = project.Resources.GetByUid(1);

// ResourceWork의 시간 단계 데이터를 출력합니다.
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// ResourceCost의 시간 단계 데이터를 출력합니다.
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


