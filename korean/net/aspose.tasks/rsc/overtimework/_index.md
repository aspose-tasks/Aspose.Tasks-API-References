---
title: "Rsc.OvertimeWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 작업에서 수행하도록 예정된 초과 근무량이며, 관련 리소스의 초과 근무 요율로 청구됩니다."
type: docs
weight: 530
url: /ko/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

작업에서 리소스가 수행하도록 예정된 초과 근무량이며, 관련 리소스의 초과 근무율에 따라 청구됩니다.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
```

## 예제

리소스 초과 근무 값을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// 모든 리소스에 대한 초과 근무 관련 매개변수를 표시합니다.
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


