---
title: "PageSettings.PercentOfNormalSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageSettings प्रॉपर्टी। सामान्य आकार का प्रतिशत प्राप्त करता है या सेट करता है जिससे प्रिंटिंग को समायोजित किया जा सके"
type: docs
weight: 90
url: /hi/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत प्राप्त करता है या सेट करता है।

```csharp
public int PercentOfNormalSize { get; set; }
```

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


