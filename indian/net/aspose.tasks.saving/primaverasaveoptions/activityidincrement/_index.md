---
title: "PrimaveraSaveOptions.ActivityIdIncrement"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraSaveOptions प्रॉपर्टी। सक्रियता IDs को पुनः क्रमांकित करने में उपयोग किए जाने वाले वृद्धि को प्राप्त करता है या सेट करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/primaverasaveoptions/activityidincrement/
---
## PrimaveraSaveOptions.ActivityIdIncrement property

एक्टिविटी IDs को री-नंबर करने में उपयोग होने वाले इन्क्रिमेंट को प्राप्त करता है या सेट करता है।

```csharp
public int ActivityIdIncrement { get; set; }
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


