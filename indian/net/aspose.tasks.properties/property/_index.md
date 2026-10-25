---
title: "क्लास प्रॉपर्टी"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Properties.Property क्लास। एक प्रॉपर्टी की बेस क्लास को दर्शाता है"
type: docs
weight: 1580
url: /hi/net/aspose.tasks.properties/property/
---
## Property class

एक प्रॉपर्टी की बेस क्लास का प्रतिनिधित्व करता है।

```csharp
public abstract class Property
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | प्रॉपर्टी का नाम प्राप्त करता है। |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | प्रॉपर्टी का मान प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | प्रॉपर्टी का मान स्ट्रिंग के रूप में लौटाता है। |

## उदाहरण

दिखाता है कि प्रोजेक्ट की बिल्ट‑इन प्रॉपर्टीज़ को कैसे पढ़ा जाए।

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// बिल्ट‑इन प्रॉपर्टी संग्रह पर इटरेट करें
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### संबंधित देखें

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


