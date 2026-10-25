---
title: "NullableBool.op_Implicit"
second_title: "Aspose.Tasks for .NET API 참조"
description: "NullableBool 메서드. NullableBool 인스턴스를 부울 값으로 암시적으로 변환합니다. Value가 true이고 IsDefined가 true일 때 true를 반환합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

[`NullableBool`](../) 인스턴스를 부울 값으로 암시적으로 변환합니다. [`Value`](../value/)가 true이고 [`IsDefined`](../isdefined/)가 true일 때 true를 반환합니다.

```csharp
public static implicit operator bool(NullableBool val)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | NullableBool | 변환할 값. |

### 반환 값

부울 값.

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

## implicit operator {#op_implicit}

부울 값을 [`NullableBool`](../) 인스턴스로 암시적으로 변환합니다.

```csharp
public static implicit operator NullableBool(bool val)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | Boolean | 변환할 값. |

### 반환 값

변환된 [`NullableBool`](../) 인스턴스.

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


