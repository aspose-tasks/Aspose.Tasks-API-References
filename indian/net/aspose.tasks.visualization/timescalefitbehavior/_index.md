---
title: "एनम TimescaleFitBehavior"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.TimescaleFitBehavior एनम। टाइमस्केल क्षेत्र को पेज की चौड़ाई के साथ संरेखित करने के लिए उपयोग किए जाने वाले व्यवहार का प्रतिनिधित्व करता है"
type: docs
weight: 3440
url: /hi/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

टाइमस्केल क्षेत्र को पृष्ठ की चौड़ाई के साथ संरेखित करने के लिए उपयोग किए जाने वाले व्यवहार का प्रतिनिधित्व करता है।

```csharp
public enum TimescaleFitBehavior
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| DefinedInView | `0` | कैलेंडर सेक्शन को रेंडर किए गए व्यू की View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage प्रॉपर्टी के अनुसार रेंडर किया जाता है। |
| NoScaleToEndDate | `1` | कैलेंडर सेक्शन को ठीक EndDate तक रेंडर किया जाता है, भले ही पेज पर खाली जगह हो। |
| NoScaleToEndOfPage | `2` | कैलेंडर सेक्शन को अंतिम पेज के अंत (दाएँ पक्ष) तक रेंडर किया जाता है। इसलिए अंतिम रेंडर की गई तिथि EndDate से अधिक हो सकती है। |
| ScaleToEndOfPage | `3` | रेंडरिंग इंजन तिथियों को इस प्रकार संरेखित करने का प्रयास करेगा कि EndDate अंतिम पेज के अंत (दाएँ पक्ष) के साथ संरेखित हो। यह MS Project के "Page Setup \ View \ Fit timescale to end of page" विकल्प के सक्षम होने के अनुरूप है। |

## उदाहरण

दिखाता है कि TimescaleFitBehavior का उपयोग करके Gantt चार्ट का टाइमस्केल अंतिम पेज के अंत तक कैसे फिट करें।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


