---
title: "क्लास TableField"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TableField क्लास। प्रोजेक्ट में तालिका के एक फ़ील्ड का प्रतिनिधित्व करता है"
type: docs
weight: 2340
url: /hi/net/aspose.tasks/tablefield/
---
## TableField class

प्रोजेक्ट में तालिका के एक फ़ील्ड का प्रतिनिधित्व करता है।

```csharp
public class TableField
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TableField](tablefield/)() | `TableField` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | तालिका फ़ील्ड में डेटा की संरेखण को प्राप्त करता है या सेट करता है। |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | तालिका फ़ील्ड में शीर्षक की संरेखण को प्राप्त करता है या सेट करता है। |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | तालिका फ़ील्ड के प्रकार को प्राप्त करता है या सेट करता है। |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | तालिका में फ़ील्ड के शीर्षक को प्राप्त करता है या सेट करता है। |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | तालिका में फ़ील्ड कॉलम की चौड़ाई (पॉइंट्स में) को प्राप्त करता है या सेट करता है। |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | तालिका कॉलम हेडिंग को कई पंक्तियों में रैप करने की अनुमति है या कॉलम की चौड़ाई से अधिक होने पर उसे ट्रंकेट करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | कॉलम टेक्स्ट को कई लाइनों में रैप करने या जब यह कॉलम की चौड़ाई से अधिक हो जाए तो उसे ट्रंकेट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। MSP 2010 संस्करण और बाद के संस्करणों द्वारा समर्थित। |

## उदाहरण

प्रोजेक्ट के व्यू के साथ काम करने और डिफ़ॉल्ट व्यू में कॉलम जोड़ने का तरीका दिखाता है (जो MPP फ़ाइल को MS Project में खोलने पर दिखाया जाता है)।

```csharp
// व्यूज़ के बिना एक खाली प्रोजेक्ट बनाएं
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// डिफ़ॉल्ट व्यू को संशोधित करें (यह एक गैंट चार्ट व्यू है)।
// या आप प्रोजेक्ट.View संग्रह का उपयोग करके व्यू को नाम से या व्यू स्क्रीन से चुन सकते हैं।
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// WriteViewData फ़्लैग का उपयोग व्यू की प्रॉपर्टीज़ में किए गए बदलावों को स्थायी बनाने के लिए किया जाना चाहिए।
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


