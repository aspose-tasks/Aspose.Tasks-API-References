---
title: "Enum Timescale"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.Timescale enum. विकल्पों को परिभाषित करता है जो यह निर्दिष्ट करते हैं कि प्रोजेक्ट को ग्राफिक फ़ॉर्मेट में निर्यात करने पर गैंट चार्ट टास्क उपयोग या रिसोर्स उपयोग व्यूज़ में टाइमस्केल कैसे रेंडर किया जाए।"
type: docs
weight: 3430
url: /hi/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

परियोजना को ग्राफिक फ़ॉर्मेट में निर्यात करने पर Gantt Chart, Task Usage या Resource Usage दृश्यों में टाइमस्केल को कैसे रेंडर किया जाए, यह निर्धारित करने वाले विकल्पों को परिभाषित करता है।

```csharp
public enum Timescale
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| DefinedInView | `0` | प्रोजेक्ट व्यू की प्रॉपर्टीज़ में परिभाषित टाइमस्केल सेटिंग्स का उपयोग करें: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). यह उन फ़ॉर्मेट्स के लिए मान्य है जिनमें व्यू डेटा शामिल है। उदाहरण के लिए, MPP फ़ॉर्मेट से पढ़े गए प्रोजेक्ट्स। |
| Days | `1` | पहले से परिभाषित दो-स्तरीय टाइमस्केल जहाँ न्यूनतम विवरण स्तर एक दिन है। |
| ThirdsOfMonths | `10` | पहले से परिभाषित दो-स्तरीय टाइमस्केल जहाँ विवरण स्तर महीने का एक तिहाई है। |
| Months | `30` | पहले से परिभाषित दो-स्तरीय टाइमस्केल जहाँ न्यूनतम विवरण स्तर एक महीना है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


