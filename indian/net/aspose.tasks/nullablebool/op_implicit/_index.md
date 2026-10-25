---
title: "NullableBool.op_Implicit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "NullableBool मेथड। एक NullableBool इंस्टेंस को बूलियन मान में अप्रत्यक्ष रूप से परिवर्तित करता है। जब Value true और IsDefined true हो तो true लौटाता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

एक [`NullableBool`](../) इंस्टेंस को बूलियन मान में अप्रत्यक्ष रूप से परिवर्तित करता है। जब [`Value`](../value/) true और [`IsDefined`](../isdefined/) true हो तो true लौटाता है।

```csharp
public static implicit operator bool(NullableBool val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | NullableBool | परिवर्तित करने के लिए मान। |

### रिटर्न वैल्यू

एक बूलियन मान।

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.NullableBool" /&gt; इंस्टेंस की तुलना कैसे करें।

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// बूल्स की समानता को 'IsDefined' और 'Value' प्रॉपर्टीज़ के विरुद्ध जाँच किया जाता है।
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// अप्रत्यक्ष रूप से बूल में परिवर्तन की जाँच करता है: bool1 True है क्योंकि यह परिभाषित है और Value True पर सेट है।
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// अप्रत्यक्ष रूप से बूल में परिवर्तन की जाँच करता है: bool2 False है क्योंकि यह परिभाषित नहीं है।
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// अप्रत्यक्ष रूप से बूल में परिवर्तन की जाँच करता है
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### संबंधित देखें

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## implicit operator {#op_implicit}

बूलियन मान को अप्रत्यक्ष रूप से [`NullableBool`](../) इंस्टेंस में परिवर्तित करता है।

```csharp
public static implicit operator NullableBool(bool val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | Boolean | परिवर्तित करने के लिए मान। |

### रिटर्न वैल्यू

परिवर्तित [`NullableBool`](../) इंस्टेंस।

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.NullableBool" /&gt; इंस्टेंस की तुलना कैसे करें।

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// बूल्स की समानता को 'IsDefined' और 'Value' प्रॉपर्टीज़ के विरुद्ध जाँच किया जाता है।
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// अप्रत्यक्ष रूप से बूल में परिवर्तन की जाँच करता है: bool1 True है क्योंकि यह परिभाषित है और Value True पर सेट है।
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// अप्रत्यक्ष रूप से बूल में परिवर्तन की जाँच करता है: bool2 False है क्योंकि यह परिभाषित नहीं है।
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// अप्रत्यक्ष रूप से बूल में परिवर्तन की जाँच करता है
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### संबंधित देखें

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


