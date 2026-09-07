---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। गैर-कार्य समय का रंग प्राप्त करता है या सेट करता है।"
type: docs
weight: 110
url: /hi/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

गैर-कार्य समय का रंग प्राप्त करता है या सेट करता है।

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## उदाहरण

दिखाता है कि कैसे गैर-कार्य समय के लिए कस्टम रंग सेट किया जाए।

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### संबंधित देखें

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


