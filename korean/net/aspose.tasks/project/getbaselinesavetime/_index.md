---
title: "Project.GetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 기준 저장 시간을 반환합니다."
type: docs
weight: 1090
url: /ko/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

기준선 저장 시간을 반환합니다.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| baselineNumber | BaselineType | 베이스라인 번호 [`BaselineType`](../../baselinetype/). |

### 반환 값

베이스라인의 마지막 저장 날짜와 시간입니다.

## 비고

기준이 저장되지 않은 경우 DateTime.MinValue를 반환합니다.

## 예제

프로젝트의 베이스라인 저장 시간을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// 베이스라인 저장 시간 설정
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### 또 보기

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


