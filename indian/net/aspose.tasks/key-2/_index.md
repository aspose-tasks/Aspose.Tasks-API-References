---
title: "संरचना KeyTK"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Key2TK struct. निर्दिष्ट प्रकार की क्लास की प्रॉपर्टी कुंजी का प्रतिनिधित्व करता है। इस क्लास का एक इंस्टेंस कंटेनर की प्रॉपर्टी प्राप्त करने या सेट करने के समय उपयोग किया जाता है।"
type: docs
weight: 930
url: /hi/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

निर्दिष्ट प्रकार की क्लास की प्रॉपर्टी कुंजी का प्रतिनिधित्व करता है। इस क्लास का एक इंस्टेंस कंटेनर की प्रॉपर्टी प्राप्त करने या सेट करने के समय उपयोग किया जाता है।

```csharp
public struct Key<T, K>
    where K : struct
```

| पैरामीटर | विवरण |
| --- | --- |
| T | प्रॉपर्टी मान का प्रकार। |
| K | प्रॉपर्टी कुंजी का प्रकार। |

## गुण

| नाम | विवरण |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | प्रॉपर्टी की कुंजी प्राप्त करता है। |

## उदाहरण

Prj.ActualsInSync प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


