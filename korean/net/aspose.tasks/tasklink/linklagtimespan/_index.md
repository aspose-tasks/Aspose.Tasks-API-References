---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLink 속성. LagFormat에 따라 지연 기간을 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

LagFormat에 따라 지연 지속 시간을 가져오거나 설정합니다.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | LagFormat이 TimeUnitType.Percent인 TaskLink의 값을 설정하려고 할 때. |

## 비고

링크 지연은 백분율 값(LagFormat이 TimeUnitType.Percent)일 수 있습니다. 이 경우 기간은 PredTask 기간의 백분율로 계산됩니다. 그렇지 않으면 메서드는 TaskLink의 지연을 나타내는 TimeSpan 값을 반환합니다.

### 또 보기

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


