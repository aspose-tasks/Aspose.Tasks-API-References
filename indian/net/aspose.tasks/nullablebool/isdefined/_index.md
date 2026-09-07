---
title: "NullableBool.IsDefined"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "NullableBool प्रॉपर्टी। यह एक मान प्राप्त करता है जो दर्शाता है कि मान परिभाषित था या नहीं, अन्यथा false"
type: docs
weight: 20
url: /hi/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

एक मान प्राप्त करता है जो दर्शाता है कि मान परिभाषित था या नहीं; अन्यथा, false.

```csharp
public bool IsDefined { get; }
```

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


