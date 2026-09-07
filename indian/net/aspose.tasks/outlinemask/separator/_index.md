---
title: "OutlineMask.Separator"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineMask property. कोड मानों के विभाजक को प्राप्त करता है या सेट करता है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/outlinemask/separator/
---
## OutlineMask.Separator property

कोड मानों के विभाजक को प्राप्त करता है या सेट करता है।

```csharp
public string Separator { get; set; }
```

## उदाहरण

आउटलाइन मास्क के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// मास्क का प्रकार सेट करें
mask.Type = MaskType.Characters;

// कोड मानों का विभाजक सेट करें
mask.Separator = "/";

// मास्क का स्तर सेट करें
mask.Level = 1;

// आउटलाइन कोड मानों की अधिकतम लंबाई (अक्षरों में) सेट करें। यदि लंबाई परिभाषित नहीं है तो 0।
mask.Length = 2;

// परिभाषा में मास्क जोड़ें
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### संबंधित देखें

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


