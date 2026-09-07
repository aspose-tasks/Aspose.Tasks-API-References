---
title: "क्लास PageMargins"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PageMargins क्लास। प्रिंटिंग के लिए पेज मार्जिन का प्रतिनिधित्व करता है"
type: docs
weight: 3230
url: /hi/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

प्रिंटिंग के लिए पेज मार्जिन को दर्शाता है।

```csharp
public class PageMargins
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageMargins](pagemargins/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | बॉर्डर प्रिंट करने की स्थिति प्राप्त करता है या सेट करता है। यह [`Border`](../border/) एनीमरेशन के मानों में से एक हो सकता है। |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | सेमी में नीचे मार्जिन का आकार प्राप्त करता है या सेट करता है। |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | सेमी में बाएँ मार्जिन का आकार प्राप्त करता है या सेट करता है। |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | सेमी में दाएँ मार्जिन का आकार प्राप्त करता है या सेट करता है। |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | सेमी में ऊपर मार्जिन का आकार प्राप्त करता है या सेट करता है। |

## उदाहरण

पेज मार्जिन के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// डिफ़ॉल्ट व्यू को संशोधित करने देता है
var margins = project.DefaultView.PageInfo.Margins;

// मार्जिन को संशोधित करने देता है
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


