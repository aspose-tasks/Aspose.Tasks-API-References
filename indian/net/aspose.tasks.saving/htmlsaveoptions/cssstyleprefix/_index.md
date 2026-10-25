---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "HtmlSaveOptions प्रॉपर्टी। CSS स्टाइल प्रीफ़िक्स प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

CSS स्टाइल प्रीफ़िक्स को प्राप्त करता है या सेट करता है।

```csharp
public string CssStylePrefix { get; set; }
```

## उदाहरण

दिखाता है कि HTML में निर्यात के दौरान उपयोग किए जाने वाले CSS स्टाइल्स के लिए सामान्य प्रीफ़िक्स कैसे सेट करें।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### संबंधित देखें

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


