---
title: "क्लास BuiltInProjectPropertyCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Properties.BuiltInProjectPropertyCollection क्लास। बिल्ट‑इन प्रोजेक्ट प्रॉपर्टीज़ का संग्रह दर्शाता है"
type: docs
weight: 1530
url: /hi/net/aspose.tasks.properties/builtinprojectpropertycollection/
---
## BuiltInProjectPropertyCollection class

अंतर्निहित प्रोजेक्ट प्रॉपर्टीज़ का संग्रह दर्शाता है।

```csharp
public sealed class BuiltInProjectPropertyCollection : 
    PropertyKeyedCollection<BuiltInProjectProperty>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Author](../../aspose.tasks.properties/builtinprojectpropertycollection/author/) { get; set; } | प्रोजेक्ट के लेखक को प्राप्त करता है या सेट करता है। |
| [Category](../../aspose.tasks.properties/builtinprojectpropertycollection/category/) { get; set; } | प्रोजेक्ट की श्रेणी को प्राप्त करता है या सेट करता है। |
| [Comments](../../aspose.tasks.properties/builtinprojectpropertycollection/comments/) { get; set; } | प्रोजेक्ट की टिप्पणियों को प्राप्त करता है या सेट करता है। |
| [Company](../../aspose.tasks.properties/builtinprojectpropertycollection/company/) { get; set; } | प्रोजेक्ट की कंपनी को प्राप्त करता है या सेट करता है। |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| [HyperlinkBase](../../aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/) { get; set; } | प्रोजेक्ट के हाइपरलिंक बेस को प्राप्त करता है या सेट करता है। |
| override [IsReadOnly](../../aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Keywords](../../aspose.tasks.properties/builtinprojectpropertycollection/keywords/) { get; set; } | प्रोजेक्ट के कीवर्ड्स को प्राप्त करता है या सेट करता है। |
| [Manager](../../aspose.tasks.properties/builtinprojectpropertycollection/manager/) { get; set; } | प्रोजेक्ट के मैनेजर को प्राप्त करता है या सेट करता है। |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |
| [Subject](../../aspose.tasks.properties/builtinprojectpropertycollection/subject/) { get; set; } | प्रोजेक्ट के विषय को प्राप्त करता है या सेट करता है। |
| [Title](../../aspose.tasks.properties/builtinprojectpropertycollection/title/) { get; set; } | प्रोजेक्ट का शीर्षक प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(BuiltInProjectProperty) |  |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [BuiltInProjectProperty](../builtinprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


