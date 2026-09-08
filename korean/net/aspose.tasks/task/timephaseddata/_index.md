---
title: "Task.TimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 이 작업의 TimephasedDataCollection 객체를 가져오거나 설정합니다. 작업과 연결된 시간 구분 데이터 블록"
type: docs
weight: 1220
url: /ko/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

이 작업의 TimephasedDataCollection 객체를 가져오거나 설정합니다. 작업과 연결된 시간 단계 데이터 블록입니다.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## 비고

XML 형식에 대해서만 읽기가 지원됩니다.

## 예제

작업의 시간 구분 데이터를 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
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


