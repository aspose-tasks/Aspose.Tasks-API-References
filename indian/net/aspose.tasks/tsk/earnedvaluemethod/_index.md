---
title: "Tsk.EarnedValueMethod"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि बजटेड लागत ऑफ वर्क परफ़ॉर्म्ड (BCWP) की गणना के लिए Complete या Physical Complete फ़ील्ड में से कौन सा उपयोग किया जाना चाहिए"
type: docs
weight: 350
url: /hi/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

% पूर्ण या भौतिक % पूर्ण फ़ील्ड का उपयोग किया जाना चाहिए या नहीं, यह निर्धारित करता है ताकि किए गए कार्य की बजटेड लागत (BCWP) की गणना की जा सके।

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## उदाहरण

दिखाता है कि Tsk.EarnedValueMethod प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


