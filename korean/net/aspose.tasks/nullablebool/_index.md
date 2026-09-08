---
title: "구조체 NullableBool"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.NullableBool struct. 정의되었는지 여부를 확인할 수 있는 부울 값용 클래스"
type: docs
weight: 1110
url: /ko/net/aspose.tasks/nullablebool/
---
## NullableBool structure

값이 정의되었는지 여부를 확인할 수 있는 부울 값용 클래스입니다.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | 지정된 부울 값을 사용하여 `NullableBool` 구조체의 새 인스턴스를 초기화합니다. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | `NullableBool` 구조체의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | 값이 정의되었는지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | 현재 값이 true인지 false인지 나타내는 값을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | 이 인스턴스가 `NullableBool` 클래스의 지정된 인스턴스와 같은지 여부를 나타내는 플래그를 반환합니다. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그를 반환합니다. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | `NullableBool` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | 현재 객체를 나타내는 문자열을 반환합니다. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | `NullableBool` 인스턴스를 암시적으로 부울 값으로 변환합니다. [`Value`](./value/)가 true이고 [`IsDefined`](./isdefined/)가 true일 때 true를 반환합니다. (2 연산자) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |

## 예제

다음과 같이 &lt;see cref=\"NullableBool\" /&gt; 클래스를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 어디에서 <see cref=\"Aspose.Tasks.NullableBool\" /> 클래스가 사용되는지 확인해 보겠습니다
// <see cref=\"Aspose.Tasks.NullableBool\" />의 주요 장점은 
// 구성을 통해 이를 정의되지 않음으로 설정할 수 있습니다
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// nullable bool 인스턴스를 사용합니다
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// nullable bool 인스턴스를 사용합니다
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


