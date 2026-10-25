---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 지정된 날짜/시간 구간에 대한 시간별 작업량을 가져옵니다."
type: docs
weight: 730
url: /ko/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

지정된 날짜/시간 구간에 대한 시간 구분 작업량을 가져옵니다.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 날짜/시간 구간의 시작. |
| 끝 | DateTime | 날짜/시간 구간의 끝. |
| timephasedDataType | TimephasedDataType | 사용할 시간별 데이터의 유형. |

## 예제

임의의 날짜/시간 구간에 대한 할당 작업을 계산하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// 각 시간별 할당 작업을 출력합니다.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### 또 보기

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

지정된 날짜/시간 구간에 대한 시간 구분 작업량을 가져옵니다.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 날짜/시간 구간의 시작. |
| 끝 | DateTime | 날짜/시간 구간의 끝. |

### 또 보기

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


