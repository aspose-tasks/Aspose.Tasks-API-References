---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfSaveOptions कंस्ट्रक्टर। एक नया PdfSaveOptions क्लास का इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग दस्तावेज़ को PDF फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

[`PdfSaveOptions`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग दस्तावेज़ को [`PDF`](../../savefileformat/) फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।

```csharp
public PdfSaveOptions()
```

## उदाहरण

दिखाता है कि प्रोजेक्ट के चयनित पेजों को PDF फ़ाइल में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// आइए जांचते हैं कि कितने पेज निर्यात किए जा सकते हैं
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### संबंधित देखें

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


