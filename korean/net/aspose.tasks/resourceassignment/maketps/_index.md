---
title: "ResourceAssignment.MakeTPs"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 시간 단계 데이터 목록을 생성합니다"
type: docs
weight: 740
url: /ko/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

시간 구분 데이터를 목록으로 생성합니다.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | DateTime | 지정된 시작 날짜. |
| 시간 | TimeSpan | 지정된 작업 시간. |
| 캘린더 | Calendar | 지정된 작업 캘린더. |
| 목록 | List`1 | 시간 단계 데이터 목록. |
| isWorking | Boolean | 지정된 플래그는 시간 단계 데이터가 작업 중인지 여부를 지정합니다. |
| type | Int32 | 지정된 시간 단계 데이터 유형. |

### 반환 값

목록이 비어 있으면 목록의 최대 날짜 또는 시작 날짜.

## 예제

매개변수를 사용하여 TP를 생성하는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### 또 보기

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


