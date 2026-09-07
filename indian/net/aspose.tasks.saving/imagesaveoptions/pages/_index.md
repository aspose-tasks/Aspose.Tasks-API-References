---
title: "ImageSaveOptions.Pages"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions प्रॉपर्टी। प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजते समय सहेजने के लिए पृष्ठ संख्याओं की सूची को प्राप्त करता है या सेट करता है। यदि यह सूची खाली है तो सभी पृष्ठ सहेजे जाएंगे"
type: docs
weight: 50
url: /hi/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पेज नंबरों की सूची प्राप्त करता है या सेट करता है। यदि यह सूची खाली है तो सभी पेज सहेजे जाएंगे।

```csharp
public List<int> Pages { get; set; }
```

## उदाहरण

दिखाता है कि चयनित पेजों को छवि के रूप में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### संबंधित देखें

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


