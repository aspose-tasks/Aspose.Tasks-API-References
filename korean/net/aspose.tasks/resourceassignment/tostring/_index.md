---
title: "ResourceAssignment.ToString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. ResourceAssignment 클래스 인스턴스의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다."
type: docs
weight: 790
url: /ko/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

`[`ResourceAssignment`](../)` 클래스 인스턴스의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다.

```csharp
public override string ToString()
```

### 반환 값

할당 객체를 나타내는 짧은 문자열.

## 예제

일반 할당 정보를 출력하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // 작업 할당을 표시합니다.
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### 또 보기

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


