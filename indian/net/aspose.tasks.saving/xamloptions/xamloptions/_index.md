---
title: "XamlOptions.XamlOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "XamlOptions कंस्ट्रक्टर। XamlOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसे प्रोजेक्ट को XAML फ़ॉर्मेट में सहेजने के लिए उपयोग किया जा सकता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

[`XamlOptions`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसे प्रोजेक्ट को XAML फ़ॉर्मेट में सहेजने के लिए उपयोग किया जा सकता है।

```csharp
public XamlOptions()
```

## उदाहरण

सेव विकल्पों का उपयोग करके XAML फ़ॉर्मेट में प्रोजेक्ट को कैसे सेव किया जाए, यह दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### संबंधित देखें

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


