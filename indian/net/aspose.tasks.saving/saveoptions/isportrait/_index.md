---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो यह false लौटाता है।"
type: docs
weight: 70
url: /hi/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि पेज अभिविन्यास पोर्ट्रेट है; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है।

```csharp
public bool IsPortrait { get; set; }
```

## टिप्पणियाँ

जब SaveOptions.PageSize == Visualization.PageSize.DefinedInView हो तो यह लागू नहीं होता। इस स्थिति में View.PageInfo.PageSettings.IsPortrait का उपयोग किया जाता है। जब SaveOptions.CustomPageSize सेट किया जाता है तो यह लागू नहीं होता।

## उदाहरण

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


