---
title: "SaveOptions.PageCount"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। प्राप्त करता है या सेट करता है प्रोजेक्ट के पृष्ठों की संख्या।"
type: docs
weight: 120
url: /hi/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

प्रोजेक्ट के पृष्ठों की संख्या प्राप्त करता है या सेट करता है।

```csharp
public int PageCount { get; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


