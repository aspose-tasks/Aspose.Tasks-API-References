---
title: "Prj.ActualsInSync"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि सभी वास्तविक कार्यों को परियोजना के साथ सिंक्रनाइज़ किया गया है या नहीं"
type: docs
weight: 10
url: /hi/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

निर्धारित करता है कि सभी वास्तविक कार्यों को परियोजना के साथ समन्वयित किया गया है या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## उदाहरण

Prj.ActualsInSync प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


