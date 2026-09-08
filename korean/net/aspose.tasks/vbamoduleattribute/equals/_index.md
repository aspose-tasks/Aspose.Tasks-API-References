---
title: "VbaModuleAttribute.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaModuleAttribute 메서드. 이 인스턴스가 지정된 VbaModuleAttribute 객체와 같은지 여부를 나타내는 값을 반환합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

이 인스턴스가 지정된 [`VbaModuleAttribute`](../) 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | VbaModuleAttribute | 이 인스턴스와 비교할 지정된 [`VbaModuleAttribute`](../) 객체입니다. |

### 반환 값

이 인스턴스가 지정된 [`VbaModuleAttribute`](../) 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

## 예제

VBA 모듈 속성의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### 또 보기

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 [`VbaModuleAttribute`](../) 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 지정된 [`VbaModuleAttribute`](../) 객체입니다. |

### 반환 값

이 인스턴스가 지정된 [`VbaModuleAttribute`](../) 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

## 예제

VBA 모듈 속성의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### 또 보기

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


