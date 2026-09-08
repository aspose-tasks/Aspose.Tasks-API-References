---
title: "NullableBool.ToString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "NullableBool 메서드. 현재 객체를 나타내는 문자열을 반환합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

현재 객체를 나타내는 문자열을 반환합니다.

```csharp
public override string ToString()
```

### 반환 값

현재 객체를 나타내는 문자열.

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


