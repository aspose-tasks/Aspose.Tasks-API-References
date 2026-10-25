---
title: "NullableBool.NullableBool"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "NullableBool कंस्ट्रक्टर। निर्दिष्ट बूलियन मान के साथ NullableBool स्ट्रक्ट का नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

निर्दिष्ट बूलियन मान के साथ [`NullableBool`](../) स्ट्रक्ट का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public NullableBool(bool value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | Boolean | निर्दिष्ट बूलियन मान। |

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## NullableBool(bool, bool) {#constructor_1}

एक नया उदाहरण प्रारंभ करता है [`NullableBool`](../) संरचना का।

```csharp
public NullableBool(bool value, bool isDefined)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | Boolean | वर्तमान मान। |
| isDefined | Boolean | वह मान जो दर्शाता है कि वर्तमान मान परिभाषित है या नहीं। |

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


