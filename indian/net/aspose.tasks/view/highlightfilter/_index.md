---
title: "View.HighlightFilter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "View प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि Microsoft Project एकल दृश्य के लिए फ़िल्टर को हाइलाइट करता है या नहीं"
type: docs
weight: 40
url: /hi/net/aspose.tasks/view/highlightfilter/
---
## View.HighlightFilter property

Microsoft Project द्वारा एकल दृश्य के लिए फ़िल्टर को हाइलाइट करने के लिए मान प्राप्त करता है या सेट करता है।

```csharp
public bool HighlightFilter { get; set; }
```

## उदाहरण

MS Project व्यूज़ के साथ काम करने का तरीका दिखाता है।

```csharp
// व्यूज़ के बिना एक खाली प्रोजेक्ट बनाएं
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// एक मानक गैंट चार्ट व्यू बनाएं
View view = new GanttChartView();

// कुछ व्यू प्रॉपर्टीज़ सेट करें
// Microsoft Project रिबन में व्यू या अन्य व्यूज़ ड्रॉप-डाउन सूची में एकल व्यू नाम दिखाता है या नहीं, यह दर्शाने वाला मान सेट करें
view.ShowInMenu = true;
// Microsoft Project एकल व्यू के लिए फ़िल्टर को हाइलाइट करता है या नहीं, यह दर्शाने वाला मान सेट करें
view.HighlightFilter = true;

// अगली प्रॉपर्टीज़ का लेखन समर्थित नहीं है
// एकल व्यू में उपयोग किए जाने वाले फ़िल्टर को सेट करता है
view.Filter = null;
// एकल व्यू का समूह सेट करता है
view.Group = null;
// एकल व्यू की टेबल सेट करता है
view.Table = null;

// आइए कुछ व्यू सेटिंग्स को ट्यून करें
// सभी पृष्ठों पर प्रिंट होने वाले पहले कॉलमों की संख्या सेट करें
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// सभी पृष्ठों पर निर्दिष्ट संख्या में पहले कॉलम प्रिंट करने का संकेत देने वाला मान सेट करें
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// व्यू को हमारे प्रोजेक्ट में जोड़ें
project.Views.Add(view);

// project.Views में संशोधनों को स्थायी रखने के लिए WriteViewData फ़्लैग का उपयोग किया जाना चाहिए।
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// आइए नए जोड़े गए व्यू की कुछ प्रॉपर्टीज़ जांचें
// व्यू का यूनिक आइडेंटिफायर प्रिंट करें
Console.WriteLine("View Uid: " + view.Uid);
// एकल व्यू के स्क्रीन टाइप को प्रिंट करें
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### संबंधित देखें

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


