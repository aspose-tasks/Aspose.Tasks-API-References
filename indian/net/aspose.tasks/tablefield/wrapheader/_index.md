---
title: "TableField.WrapHeader"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TableField property. यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि क्या तालिका कॉलम हेडिंग कई पंक्तियों में रैप हो सकता है या यदि यह कॉलम की चौड़ाई से अधिक हो जाए तो इसे काट दिया जाना चाहिए"
type: docs
weight: 70
url: /hi/net/aspose.tasks/tablefield/wrapheader/
---
## TableField.WrapHeader property

तालिका कॉलम हेडिंग को कई पंक्तियों में रैप करने की अनुमति है या कॉलम की चौड़ाई से अधिक होने पर उसे ट्रंकेट करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है।

```csharp
public bool WrapHeader { get; set; }
```

## उदाहरण

प्रोजेक्ट टेबल्स को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// टेबल प्राप्त करें
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// सभी टेबल फ़ील्ड्स की जानकारी प्रदर्शित करें
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### संबंधित देखें

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


