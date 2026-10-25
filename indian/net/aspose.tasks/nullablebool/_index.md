---
title: "Struct NullableBool"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.NullableBool struct. बूलियन मानों के लिए एक क्लास है जिसमें यह जांचने की संभावना है कि मान परिभाषित है या नहीं"
type: docs
weight: 1110
url: /hi/net/aspose.tasks/nullablebool/
---
## NullableBool structure

बूलियन मानों के लिए एक क्लास, जिसमें यह जांचने की संभावना होती है कि मान परिभाषित है या नहीं।

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | `NullableBool` struct का एक नया इंस्टेंस निर्दिष्ट बूलियन मान के साथ इनिशियलाइज़ करता है। |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | `NullableBool` struct का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि मान परिभाषित था या नहीं; अन्यथा, false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि वर्तमान मान true है या false. |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | `NullableBool` क्लास के निर्दिष्ट इंस्टेंस के बराबर है या नहीं, यह दर्शाने वाला फ़्लैग लौटाता है। |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | एक फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | `NullableBool` क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है। |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है। |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | एक `NullableBool` इंस्टेंस को स्वचालित रूप से बूलियन मान में परिवर्तित करता है। जब [`Value`](./value/) सत्य हो और [`IsDefined`](./isdefined/) सत्य हो तो true लौटाता है। (2 ऑपरेटर) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |

## उदाहरण

दिखाता है कि &lt;see cref="NullableBool" /&gt; क्लास के साथ कैसे काम किया जाए।

```csharp
var project = new Project();

// चलो देखें कि <see cref="Aspose.Tasks.NullableBool" /> क्लास कहाँ उपयोग की गई है
//  <see cref="Aspose.Tasks.NullableBool" /> का मुख्य लाभ यह है कि 
// इसे निर्माण के दौरान अपरिभाषित सेट किया जा सकता है
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// nullable बूल इंस्टेंस का उपयोग करें
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// nullable बूल इंस्टेंस का उपयोग करें
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


