---
title: "PrimaveraSaveOptions.RenumberActivityIds"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraSaveOptions प्रॉपर्टी। प्राप्त करता है या सेट करता है एक मान जो दर्शाता है कि क्या एक्टिविटी IDs को पुनः क्रमांकित करने की आवश्यकता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

एक्टिविटी IDs को री-नंबर करने की आवश्यकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool RenumberActivityIds { get; set; }
```

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt; के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Primavera सेव विकल्प बनाएं और उन्हें ट्यून करें
var options = new PrimaveraSaveOptions
                  {
                      // एक एक्टिविटी का प्रीफ़िक्स और सफ़िक्स परिभाषित करें
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // एक्टिविटीज़ के री-नंबरिंग को नियंत्रित करें
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### संबंधित देखें

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


