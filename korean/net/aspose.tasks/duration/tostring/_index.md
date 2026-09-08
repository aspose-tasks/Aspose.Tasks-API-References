---
title: "Duration.ToString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. 이 인스턴스의 문자열 표현을 반환합니다"
type: docs
weight: 120
url: /ko/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

이 인스턴스의 문자열 표현을 반환합니다.

```csharp
public override string ToString()
```

### 반환 값

이 인스턴스의 문자열 표현입니다.

## 예제

기간을 문자열로 변환하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// 작업 기간을 가져옵니다
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### 또 보기

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


