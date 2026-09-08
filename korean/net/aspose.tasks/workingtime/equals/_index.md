---
title: "WorkingTime.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WorkingTime 메서드. 객체가 동일한지 확인합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

객체가 동일한지 확인합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 비교할 두 번째 객체. |

### 반환 값

객체가 동일하면 true, 그렇지 않으면 false.

## 예제

작업 시간 동일성을 확인하는 방법을 보여줍니다.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// 달력의 동일성은 작업 시간의 시작 및 종료 날짜와 비교하여 확인됩니다.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### 또 보기

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


