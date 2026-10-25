---
title: "Resource.TimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. 이 객체에 대한 TimephasedDataCollection 클래스의 인스턴스를 가져오거나 설정합니다"
type: docs
weight: 740
url: /ko/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

이 객체에 대해 [`TimephasedDataCollection`](../../timephaseddatacollection/) 클래스의 인스턴스를 가져오거나 설정합니다.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## 비고

XML 형식에 대해서만 읽기가 지원됩니다.

## 예제

리소스 시간별 데이터를 읽는 방법을 보여줍니다.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// 리소스의 시간별 데이터를 반복합니다.
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### 또 보기

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


