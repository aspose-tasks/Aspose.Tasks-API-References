---
title: "PageMargins.Borders"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageMargins प्रॉपर्टी। बॉर्डर प्रिंट करने की स्थिति प्राप्त करता है या सेट करता है। यह Border एन्‍युमरेशन के मानों में से एक हो सकता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

बॉर्डर प्रिंट करने की स्थिति प्राप्त करता है या सेट करता है। यह [`Border`](../../border/) enumeration के मानों में से एक हो सकता है।

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


