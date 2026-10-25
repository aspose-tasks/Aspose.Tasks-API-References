---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "HtmlSaveOptions कंस्ट्रक्टर। HtmlSaveOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

[`HtmlSaveOptions`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public HtmlSaveOptions()
```

## उदाहरण

HTML फ़ॉर्मेट में प्रोजेक्ट को सहेजने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// या

// केवल एक पृष्ठ जोड़ना (पृष्ठ संख्या 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### संबंधित देखें

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


