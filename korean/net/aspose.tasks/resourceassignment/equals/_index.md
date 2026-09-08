---
title: "ResourceAssignment.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 이 인스턴스가 지정된 ResourceAssignment 클래스 인스턴스와 같은지 여부를 나타내는 값을 반환합니다."
type: docs
weight: 690
url: /ko/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

이 인스턴스가 지정된 [`ResourceAssignment`](../) 클래스 인스턴스와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(ResourceAssignment other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | ResourceAssignment | 이 인스턴스와 비교할 지정된 [`ResourceAssignment`](../) 클래스 인스턴스입니다. |

### 반환 값

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## 예제

리소스 할당의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### 또 보기

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 객체. |

### 반환 값

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## 예제

리소스 할당의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### 또 보기

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


