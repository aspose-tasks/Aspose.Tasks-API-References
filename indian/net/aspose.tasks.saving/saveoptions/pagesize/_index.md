---
title: "SaveOptions.PageSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। पृष्ठ के आकार को प्राप्त करता है या सेट करता है जिसे रेंडर किया जाएगा। डिफ़ॉल्ट मान PageSize.A4 है।"
type: docs
weight: 130
url: /hi/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

रेंडर किए जाने वाले पेज का आकार प्राप्त करता है या सेट करता है (डिफ़ॉल्ट मान PageSize.A4 है)।

```csharp
public PageSize PageSize { get; set; }
```

## उदाहरण

दिखाता है कि कैसे पृष्ठ आकार सेट किया जाए (यह &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt; एनेमरेशन के मानों में से एक हो सकता है)।

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// प्रोजेक्ट को सभी प्री-डिफाइंड पृष्ठ आकारों पर रेंडर करें।
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### संबंधित देखें

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


