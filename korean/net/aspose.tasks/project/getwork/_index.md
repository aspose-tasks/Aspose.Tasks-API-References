---
title: "Project.GetWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 지정된 Double 값과 기본 작업 형식으로 Duration 객체를 가져옵니다"
type: docs
weight: 1130
url: /ko/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

지정된 Double 값과 기본 작업 형식으로 [`Duration`](../../duration/) 객체를 가져옵니다.

```csharp
public Duration GetWork(double val)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | Double | 지정된 double 값. |

### 반환 값

Duration 객체.

## 비고

이 메서드는 Project.WorkFormat 설정에 따라 다른 기간을 반환하므로 주의해서 사용해야 합니다. 예를 들어, GetWork(1.0)은 Project.WorkFormat이 TimeUnitType.Hour인 경우 1시간을, TimeUnitType.Day인 경우 1일을 반환합니다.

## 예제

기본 작업 형식으로 작업을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// 프로젝트의 기본 작업 형식으로 작업 값을 생성합니다
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### 또 보기

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


