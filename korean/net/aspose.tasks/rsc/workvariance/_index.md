---
title: "Rsc.WorkVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스의 기준 작업량과 현재 예정된 작업량 사이의 차이"
type: docs
weight: 710
url: /ko/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

리소스의 기준 작업과 현재 예정 작업 사이의 차이.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## 예제

리소스 작업 차이를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


