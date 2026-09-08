---
title: "NullableBool.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "NullableBool 메서드. NullableBool 클래스 인스턴스에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

[`NullableBool`](../) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

&lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.GetHashCode 메서드를 사용하는 방법을 보여줍니다.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool의 해시 코드는 'IsDefined' 및 'Value' 속성을 기반으로 합니다.
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### 또 보기

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


