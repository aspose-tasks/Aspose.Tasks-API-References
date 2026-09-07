---
title: "PageMargins.Top"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageMargins प्रॉपर्टी। शीर्ष मार्जिन का आकार सेंटीमीटर में प्राप्त करता है या सेट करता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks.visualization/pagemargins/top/
---
## PageMargins.Top property

सेमी में ऊपर मार्जिन का आकार प्राप्त करता है या सेट करता है।

```csharp
public double Top { get; set; }
```

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

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


