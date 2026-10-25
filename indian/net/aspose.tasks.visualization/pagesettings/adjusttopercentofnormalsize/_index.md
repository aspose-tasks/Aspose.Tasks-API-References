---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageSettings प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि क्या प्रिंटिंग को सामान्य आकार के निर्दिष्ट प्रतिशत PercentOfNormalSize पर समायोजित किया जाए।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि क्या प्रिंटिंग को सामान्य आकार के निर्दिष्ट प्रतिशत ([`PercentOfNormalSize`](../percentofnormalsize/)) पर समायोजित किया जाए।

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## टिप्पणियाँ

जब प्रोजेक्ट को HTML फ़ॉर्मेट में रेंडर किया जाता है तो यह प्रभावी नहीं होता।

## उदाहरण

निर्दिष्ट स्केल फैक्टर के साथ व्यू को रेंडर करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// एक मान सेट करें जो दर्शाता है कि व्यू को निर्दिष्ट स्केल फैक्टर का उपयोग करके स्केल किया जाना चाहिए
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// स्केल फैक्टर निर्दिष्ट करें
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### संबंधित देखें

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


