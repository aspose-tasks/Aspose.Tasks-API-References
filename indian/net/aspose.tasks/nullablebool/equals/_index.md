---
title: "NullableBool.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "NullableBool मेथड। यह एक फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस NullableBool क्लास के निर्दिष्ट इंस्टेंस के बराबर है या नहीं"
type: docs
weight: 40
url: /hi/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

एक फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस [`NullableBool`](../) क्लास के निर्दिष्ट इंस्टेंस के बराबर है या नहीं।

```csharp
public bool Equals(NullableBool other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| अन्य | NullableBool | इस इंस्टेंस की तुलना के लिए निर्दिष्ट ऑब्जेक्ट। |

### रिटर्न वैल्यू

एक फ़्लैग जो दर्शाता है कि यह इंस्टेंस [`NullableBool`](../) क्लास के निर्दिष्ट इंस्टेंस के बराबर है या नहीं।

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

## Equals(object) {#equals_1}

एक फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | इस इंस्टेंस की तुलना के लिए निर्दिष्ट ऑब्जेक्ट। |

### रिटर्न वैल्यू

एक संकेतक जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

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


