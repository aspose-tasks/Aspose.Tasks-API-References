---
title: "Prj.MultipleCriticalPaths"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि क्या कई क्रिटिकल पाथ्स की गणना की जाती है"
type: docs
weight: 530
url: /hi/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

निर्धारित करता है कि क्या कई महत्वपूर्ण पथों की गणना की जाती है।

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## उदाहरण

दिखाता है कि Prj.MultipleCriticalPaths प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


