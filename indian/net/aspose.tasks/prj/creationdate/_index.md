---
title: "Prj.CreationDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। वह तिथि और समय जब एक प्रोजेक्ट बनाया गया था"
type: docs
weight: 130
url: /hi/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

परियोजना के निर्मित होने की तिथि और समय।

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## टिप्पणियाँ

mpp फ़ाइलों में UTC फ़ॉर्मेट में सहेजा गया। DateTime प्रकार।

## उदाहरण

दिखाता है कि Prj.CreationDate प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


