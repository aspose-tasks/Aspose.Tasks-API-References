---
title: "SvgOptions.UseGradientBrush"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SvgOptions प्रॉपर्टी. निर्धारित करता है कि प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग करना है या नहीं। वर्तमान में SVG में रेंडर करने के लिए ग्रेडिएंट ब्रश का उपयोग समर्थित नहीं है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

निर्धारित करता है कि प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग करना है या नहीं। वर्तमान में SVG में रेंडर करने के लिए ग्रेडिएंट ब्रश का उपयोग समर्थित नहीं है।

```csharp
public override bool UseGradientBrush { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को SVG फ़ाइल के रूप में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // डॉक्यूमेंट को सहेजे जाने वाले <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> को सेट करें
                            PresentationFormat = PresentationFormat.GanttChart,

                            // एक मान सेट करें जो यह दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री फिट करने के लिए बढ़ाया जाना चाहिए या नहीं
                            FitContent = true,

                            // रेंडर करने के लिए न्यूनतम समय अवधि सेट करें। डिफ़ॉल्ट मान <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see> है
                            Timescale = Timescale.ThirdsOfMonths,

                            // निर्धारित करता है कि प्रोजेक्ट लेआउट रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग करना है या नहीं
                            // वर्तमान में SVG में रेंडर करने के लिए ग्रेडिएंट ब्रश का उपयोग समर्थित नहीं है।
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### संबंधित देखें

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


