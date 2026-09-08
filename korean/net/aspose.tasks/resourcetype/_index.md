---
title: "Enum ResourceType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ResourceType 열거형. 리소스 유형을 지정합니다"
type: docs
weight: 1800
url: /ko/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

리소스 유형을 지정합니다.

```csharp
public enum ResourceType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Material | `0` | 자재 리소스 유형을 나타냅니다. |
| Work | `1` | 작업 리소스 유형을 나타냅니다. |
| Cost | `2` | 비용 리소스 유형을 나타냅니다. |

## 예제

리소스 유형 작업 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업 리소스를 추가합니다
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// 자재 리소스를 추가합니다
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// 자재 리소스를 추가합니다
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// 리소스를 사용: 작업을 생성하고, 리소스를 할당하는 등...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


