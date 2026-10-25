---
title: "Property.ToString"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Property मेथड। प्रॉपर्टी मान को स्ट्रिंग के रूप में लौटाता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.properties/property/tostring/
---
## Property.ToString method

प्रॉपर्टी का मान स्ट्रिंग के रूप में लौटाता है।

```csharp
public override string ToString()
```

### रिटर्न वैल्यू

स्ट्रिंग मान।

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

* class [Property](../)
* namespace [Aspose.Tasks.Properties](../../property/)
* assembly [Aspose.Tasks](../../../)


