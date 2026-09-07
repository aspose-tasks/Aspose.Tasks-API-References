---
title: "NullableBool.op_Inequality"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "NullableBool मेथड। यह एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है"
type: docs
weight: 90
url: /hi/net/aspose.tasks/nullablebool/op_inequality/
---
## NullableBool Inequality operator

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं।

```csharp
public static bool operator !=(NullableBool a, NullableBool b)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | NullableBool | पहला [`NullableBool`](../)। |
| b | NullableBool | दूसरा [`NullableBool`](../)। |

### रिटर्न वैल्यू

एक मान जो दर्शाता है कि यह इंस्टेंस किसी निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है.

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


