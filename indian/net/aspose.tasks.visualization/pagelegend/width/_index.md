---
title: "PageLegend.Width"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageLegend प्रॉपर्टी। लेजेंड के डिफ़ॉल्ट रूप में सेंटीमीटर में प्रोजेक्ट नाम और तिथि वाले बाएँ भाग की चौड़ाई प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

लेजेंड के बाएँ भाग (डिफ़ॉल्ट रूप से प्रोजेक्ट का नाम और तिथि शामिल) की चौड़ाई सेंटीमीटर में प्राप्त करता है या सेट करता है।

```csharp
public double Width { get; set; }
```

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentOutOfRangeException | जब 0 से कम मान सेट करने का प्रयास किया जाता है। |

## उदाहरण

पेज लेजेंड जानकारी के साथ काम करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// पेज लेजेंड जानकारी पढ़ें
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// लेजेंड का संशोधन भी समर्थित है
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


