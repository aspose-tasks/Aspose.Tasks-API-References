---
title: "NullableBool.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "NullableBool 메서드. 이 인스턴스가 NullableBool 클래스의 지정된 인스턴스와 같은지 여부를 나타내는 플래그를 반환합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

[`NullableBool`](../) 클래스의 지정된 인스턴스와 이 인스턴스가 같은지 여부를 나타내는 플래그를 반환합니다.

```csharp
public bool Equals(NullableBool other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | NullableBool | 이 인스턴스와 비교할 지정된 객체. |

### 반환 값

[`NullableBool`](../) 클래스의 지정된 인스턴스와 이 인스턴스가 같은지 여부를 나타내는 플래그.

## 예제

비교하는 방법을 보여줍니다 &lt;see cref="Aspose.Tasks.NullableBool" /&gt; 인스턴스.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool의 동일성은 'IsDefined'와 'Value' 속성을 기준으로 확인됩니다.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// bool로의 암시적 변환을 확인합니다: bool1은 정의되어 있고 Value가 True로 설정되어 있기 때문에 True입니다.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// bool로의 암시적 변환을 확인합니다: bool2는 정의되지 않았기 때문에 False입니다.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// bool로의 암시적 변환을 확인합니다
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### 또 보기

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그를 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 지정된 객체. |

### 반환 값

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그.

## 예제

비교하는 방법을 보여줍니다 &lt;see cref="Aspose.Tasks.NullableBool" /&gt; 인스턴스.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool의 동일성은 'IsDefined'와 'Value' 속성을 기준으로 확인됩니다.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// bool로의 암시적 변환을 확인합니다: bool1은 정의되어 있고 Value가 True로 설정되어 있기 때문에 True입니다.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// bool로의 암시적 변환을 확인합니다: bool2는 정의되지 않았기 때문에 False입니다.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// bool로의 암시적 변환을 확인합니다
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### 또 보기

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


