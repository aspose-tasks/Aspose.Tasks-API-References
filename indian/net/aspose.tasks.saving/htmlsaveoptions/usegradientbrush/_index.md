---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "HtmlSaveOptions प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग करना है या नहीं। वर्तमान में HTML में रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग समर्थित नहीं है।"
type: docs
weight: 160
url: /hi/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

प्रोजेक्ट लेआउट को रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। वर्तमान में HTML में रेंडर करने पर ग्रेडिएंट ब्रश का उपयोग समर्थित नहीं है।

```csharp
public override bool UseGradientBrush { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को HTML फ़ाइल में निर्यात करने के लिए कस्टम फ़ॉन्ट कैसे सेट करें।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### संबंधित देखें

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


