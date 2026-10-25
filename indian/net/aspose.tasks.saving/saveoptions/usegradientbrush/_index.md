---
title: "SaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि Gantt Chart रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं।"
type: docs
weight: 220
url: /hi/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

गैंट चार्ट को रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## टिप्पणियाँ

केवल तब लागू होता है जब Gantt चार्ट व्यू रेंडर किया जाता है।

## उदाहरण

दिखाता है कि कैसे एक मान सेट किया जाए जो यह दर्शाता है कि Gantt Chart रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं।

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### संबंधित देखें

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


