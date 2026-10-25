---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "HtmlSaveOptions प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि HTML शीर्षक में प्रोजेक्ट नाम शामिल किया जाए या नहीं।"
type: docs
weight: 120
url: /hi/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि HTML शीर्षक में प्रोजेक्ट नाम शामिल किया जाए या नहीं।

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## उदाहरण

दिखाता है कि &lt;see cref=\"P:Aspose.Tasks.Saving.HtmlSaveOptions\" /&gt; विकल्पों का उपयोग करके पेज HTML हेडर/टाइटल कैसे सेट करें।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // निर्धारित करता है कि HTML शीर्षक में प्रोजेक्ट नाम शामिल किया जाए या नहीं (डिफ़ॉल्ट रूप से true)।
    IncludeProjectNameInTitle = false,

    // निर्धारित करता है कि HTML पेज हेडर में प्रोजेक्ट नाम शामिल किया जाए या नहीं (डिफ़ॉल्ट रूप से true)।
    IncludeProjectNameInPageHeader = false,

    // निर्यात किए जाने वाले पेज सेट करें।
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### संबंधित देखें

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


