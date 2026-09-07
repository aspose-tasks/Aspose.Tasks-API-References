---
title: "PdfSaveOptions.Pages"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfSaveOptions प्रॉपर्टी। प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची प्राप्त या सेट करता है। यदि यह सूची खाली है तो सभी पृष्ठ सहेजे जाएंगे।"
type: docs
weight: 60
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पेज नंबरों की सूची प्राप्त करता है या सेट करता है। यदि यह सूची खाली है तो सभी पेज सहेजे जाएंगे।

```csharp
public List<int> Pages { get; set; }
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


