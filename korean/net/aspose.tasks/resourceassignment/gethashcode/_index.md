---
title: "ResourceAssignment.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. ResourceAssignment 클래스 인스턴스에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 710
url: /ko/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

[`ResourceAssignment`](../) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

리소스 할당의 해시 코드를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// 할당의 해시 코드를 출력합니다.
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### 또 보기

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


