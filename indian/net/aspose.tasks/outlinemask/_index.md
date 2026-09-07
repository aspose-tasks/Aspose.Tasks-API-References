---
title: "क्लास OutlineMask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OutlineMask क्लास. चार तत्वों का प्रतिनिधित्व करता है एक मास्क का जो एक रूपरेखा कोड प्रारूप को परिभाषित करता है"
type: docs
weight: 1190
url: /hi/net/aspose.tasks/outlinemask/
---
## OutlineMask class

एक मास्क के चार तत्वों को दर्शाता है जो एक रूपरेखा कोड फ़ॉर्मेट को परिभाषित करता है।

```csharp
public class OutlineMask
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OutlineMask](outlinemask/)() | `OutlineMask` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | आउटलाइन कोड मानों की अधिकतम लंबाई (अक्षरों में) प्राप्त करता है या सेट करता है। यदि लंबाई परिभाषित नहीं है तो 0। |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | मास्क के स्तर को प्राप्त करता है या सेट करता है। |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | कोड मानों के विभाजक को प्राप्त करता है या सेट करता है। |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | मास्क के प्रकार को प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


