---
title: "Prj.BaselineForEarnedValue"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड. वेरिएंस मानों की गणना के लिए उपयोग किया गया विशिष्ट बेसलाइन"
type: docs
weight: 80
url: /hi/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

वैरिएंस मानों की गणना के लिए उपयोग किया गया विशिष्ट बेसलाइन।

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## उदाहरण

दिखाता है कि Prj.BaselineForEarnedValue प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


