---
title: "Prj.RemoveFileProperties"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि सहेजने पर सभी फ़ाइल गुण हटाए जाएंगे या नहीं"
type: docs
weight: 600
url: /hi/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

निर्धारित करता है कि क्या सभी फ़ाइल गुण सहेजने पर हटाए जाएंगे।

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## उदाहरण

दिखाता है कि Prj.RemoveFileProperties प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


