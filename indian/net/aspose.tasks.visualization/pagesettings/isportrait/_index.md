---
title: "PageSettings.IsPortrait"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageSettings प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि पृष्ठ अभिविन्यास पोर्ट्रेट है; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि पेज अभिविन्यास पोर्ट्रेट है; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है।

```csharp
public bool IsPortrait { get; set; }
```

## टिप्पणियाँ

जब SaveOptions.PageSize == Visualization.PageSize.DefinedInView हो तो रेंडरिंग के दौरान लागू होता है।

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.Visualization.PageSettings" /&gt; के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// सेटिंग्स प्राप्त करें
var settings = project.DefaultView.PageInfo.PageSettings;
// कुछ गुणों को समायोजित करें
// पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान सेट करें; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है।
settings.IsPortrait = true;
// प्रिंट किए जाने वाले चौड़ाई में पृष्ठों की संख्या सेट करें।
settings.PagesInWidth = 5;
// प्रिंट किए जाने वाले ऊँचाई में पृष्ठों की संख्या सेट करें।
settings.PagesInHeight = 7;
// प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत सेट करें।
settings.PercentOfNormalSize = 200;
// कागज़ का आकार सेट करें। यह <see cref="T:Aspose.Tasks.Visualization.PrinterPaperSize" /> enumeration के मानों में से एक हो सकता है।
settings.PaperSize = PrinterPaperSize.PaperB4;
// प्रिंटिंग के लिए पहला पृष्ठ संख्या सेट करें।
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

दिखाता है कि View सेटिंग्स या SaveOptions का उपयोग करके पृष्ठ आकार और अभिविन्यास कैसे निर्दिष्ट किया जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// इस मामले में पृष्ठ आकार और अभिविन्यास view.PageInfo.PageSettings.PaperSize और view.PageInfo.PageSettings.IsPortrait प्रॉपर्टीज़ से लागू होते हैं।
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// इस मामले में पृष्ठ आकार और अभिविन्यास SaveOptions की प्रॉपर्टीज़ से लागू होते हैं।
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// इस मामले में पृष्ठ आकार SaveOptions.CustomPageSize से लागू होता है। IsPortrait प्रॉपर्टी को ध्यान में नहीं रखा जाता।
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### संबंधित देखें

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


