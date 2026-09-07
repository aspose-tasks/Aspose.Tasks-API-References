---
title: "Enum MaskType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.MaskType enum. एक मास्क के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 1000
url: /hi/net/aspose.tasks/masktype/
---
## MaskType enumeration

मास्क के प्रकार को निर्दिष्ट करता है।

```csharp
public enum MaskType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Null | `0` | नल मास्क प्रकार को दर्शाता है। |
| Numbers | `1` | संख्याओं के मास्क प्रकार को दर्शाता है। |
| UpperCaseLetters | `2` | ऊपरी केस अक्षरों के मास्क प्रकार को दर्शाता है। |
| LowerCaseLetters | `3` | निचले केस अक्षरों के मास्क प्रकार को दर्शाता है। |
| Characters | `4` | अक्षरों के मास्क प्रकार को दर्शाता है। |
| Val4 | `5` | लागत के लिए लुकअप मास्क प्रकार को दर्शाता है। |
| Val5 | `6` | तिथियों के लिए लुकअप मास्क प्रकार को दर्शाता है। |
| Val6 | `7` | अवधियों के लिए लुकअप मास्क प्रकार को दर्शाता है। |
| Val7 | `8` | संख्याओं के लिए लुकअप मास्क प्रकार को दर्शाता है। |
| Val8 | `9` | फ़्लैग्स के लिए लुकअप मास्क प्रकार को दर्शाता है। |
| Val9 | `10` | समाप्ति तिथि के लिए लुकअप मास्क प्रकार को दर्शाता है। |

## उदाहरण

दिखाता है कि आउटलाइन मास्क संग्रहों के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// आउटलाइन मास्क साफ़ करें
if (outline.Masks.Count > 0)
{
    if (!outline.Masks.IsReadOnly)
    {
        outline.Masks.Clear();
    }
}

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
var maskWrong = new OutlineMask();
maskWrong.Type = MaskType.Null;

outline.Masks.Add(mask);

// एक गलत मास्क डालें
outline.Masks.Insert(0, maskWrong);

// संग्रह के इंडेक्स एक्सेस का उपयोग करके मास्क को संपादित करें
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// इंडेक्स द्वारा एक गलत मास्क हटाएँ
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// मास्कों पर इटररेट करें
foreach (var outlineMask in outline.Masks)
{
    Console.WriteLine("Length: " + outlineMask.Length);
    Console.WriteLine("Level: " + outlineMask.Level);
    Console.WriteLine("Separator: " + outlineMask.Separator);
    Console.WriteLine("Type: " + outlineMask.Type);
}

var otherProject = new Project(DataDir + "OutlineValues2010.mpp");

var otherOutline = otherProject.OutlineCodes[0];

var masks = new OutlineMask[outline.Masks.Count];
outline.Masks.CopyTo(masks, 0);

foreach (var maskToAdd in masks)
{
    if (!otherOutline.Masks.Contains(maskToAdd))
    {
        otherOutline.Masks.Add(maskToAdd);
    }
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


