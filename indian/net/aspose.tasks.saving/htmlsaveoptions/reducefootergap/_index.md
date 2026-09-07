---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "HtmlSaveOptions प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं।"
type: docs
weight: 150
url: /hi/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं।

```csharp
public bool ReduceFooterGap { get; set; }
```

## उदाहरण

दिखाता है कि HTML आउटपुट फ़ाइलों में अंतिम कार्य और फुटर के बीच के अंतराल को घटाने के लिए मान कैसे सेट किया जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### संबंधित देखें

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


