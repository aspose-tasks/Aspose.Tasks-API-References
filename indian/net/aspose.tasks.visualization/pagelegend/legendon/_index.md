---
title: "PageLegend.LegendOn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageLegend प्रॉपर्टी। लेजेंड जहाँ दिखाई देता है, उन पृष्ठों को प्राप्त करता है या सेट करता है। यह Legend enumeration के मानों में से एक हो सकता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

लेजेंड जहाँ दिखाई देता है, उन पृष्ठों को प्राप्त करता है या सेट करता है। यह [`Legend`](../../legend/) enumeration के मानों में से एक हो सकता है।

```csharp
public Legend LegendOn { get; set; }
```

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

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


