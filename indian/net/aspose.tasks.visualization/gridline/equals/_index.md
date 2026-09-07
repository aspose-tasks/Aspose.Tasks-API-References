---
title: "Gridline.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Gridline मेथड। यह फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।"
type: docs
weight: 50
url: /hi/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

एक फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | इस इंस्टेंस की तुलना के लिए निर्दिष्ट ऑब्जेक्ट। |

### रिटर्न वैल्यू

एक संकेतक जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

## उदाहरण

ग्रिडलाइन की समानता की जाँच कैसे करें, यह दर्शाता है।

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// ग्रिडलाइन की समानता को ग्रिडलाइन प्रकार के विरुद्ध जाँचा जाता है।
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// प्रकार बदलें
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### संबंधित देखें

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


