---
title: "PageSettings.PagesInWidth"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageSettings प्रॉपर्टी। प्रिंट किए जाने वाले चौड़ाई में पृष्ठों की संख्या प्राप्त करता है या सेट करता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks.visualization/pagesettings/pagesinwidth/
---
## PageSettings.PagesInWidth property

प्रिंट किए जाने वाले चौड़ाई में पृष्ठों की संख्या प्राप्त करता है या सेट करता है।

```csharp
public int PagesInWidth { get; set; }
```

## उदाहरण

'Fit X to Y pages' विकल्प के साथ व्यू को रेंडर करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// निर्दिष्ट करें कि व्यू को ऊँचाई में 2 पृष्ठों या कम में रेंडर किया जाना चाहिए
view.PageInfo.PageSettings.PagesInHeight = 2;
// निर्दिष्ट करें कि व्यू को चौड़ाई में 1 पृष्ठ में रेंडर किया जाना चाहिए
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### संबंधित देखें

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


