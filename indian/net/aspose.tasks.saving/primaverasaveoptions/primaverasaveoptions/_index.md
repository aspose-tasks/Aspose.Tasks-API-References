---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraSaveOptions कंस्ट्रक्टर। PrimaveraSaveOptions क्लास का नया इंस्टेंस प्रारंभ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

[`PrimaveraSaveOptions`](../) क्लास का नया इंस्टेंस प्रारंभ करता है।

```csharp
public PrimaveraSaveOptions()
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


