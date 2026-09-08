---
title: "Resource.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 메서드. 이 인스턴스가 Resource 클래스의 지정된 인스턴스와 같은지 여부를 나타내는 값을 반환합니다."
type: docs
weight: 820
url: /ko/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

이 인스턴스가 [`Resource`](../) 클래스의 지정된 인스턴스와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(Resource other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | Resource | 이 인스턴스와 비교할 [`Resource`](../) 클래스의 지정된 인스턴스입니다. |

### 반환 값

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## 예제

리소스 동등성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### 또 보기

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
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

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## 예제

리소스 동등성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### 또 보기

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


