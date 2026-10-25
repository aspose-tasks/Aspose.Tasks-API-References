---
title: "Enum Border"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.Border enum. बॉर्डर के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 2970
url: /hi/net/aspose.tasks.visualization/border/
---
## Border enumeration

बॉर्डर्स के प्रकार को निर्दिष्ट करता है।

```csharp
public enum Border
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| NoBorder | `0` | कोई बॉर्डर नहीं। |
| AroundEveryPage | `1` | प्रत्येक पृष्ठ के चारों ओर। |
| OutsidePages | `2` | बाहरी पृष्ठों पर। |

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


