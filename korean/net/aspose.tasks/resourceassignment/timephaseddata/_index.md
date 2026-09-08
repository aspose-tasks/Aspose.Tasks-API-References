---
title: "ResourceAssignment.TimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 속성. TimephasedDataCollection 클래스의 인스턴스를 가져오거나 설정합니다. 이 클래스는 TimephasedData 클래스의 요소를 포함합니다."
type: docs
weight: 600
url: /ko/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

[`TimephasedDataCollection`](../../timephaseddatacollection/) 클래스의 인스턴스를 가져오거나 설정합니다. 이 클래스는 `TimephasedData` 클래스의 요소를 포함합니다.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## 예제

리소스 할당의 시간별 데이터를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
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
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// 시간별 데이터를 가져옵니다.
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


