---
title: "ResourceAssignment.Get"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 이 컨테이너에서 속성이 매핑된 값을 반환합니다"
type: docs
weight: 700
url: /ko/net/aspose.tasks/resourceassignment/get/
---
## ResourceAssignment.Get&lt;T&gt; method

이 컨테이너에서 속성이 매핑된 값을 반환합니다.

```csharp
public T Get<T>(Key<T, AsnKey> key)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 매핑된 값의 유형. |
| key | 지정된 속성 키. 속성 키를 가져오기 위한 [`Asn`](../../asn/). |

### 반환 값

속성이 이 컨테이너에 매핑되는 값.

## 예제

할당을 생성하고 일반 할당 속성을 가져오거나 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


