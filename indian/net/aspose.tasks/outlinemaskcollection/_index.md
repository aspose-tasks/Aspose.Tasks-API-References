---
title: "क्लास OutlineMaskCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OutlineMaskCollection क्लास। OutlineMask ऑब्जेक्ट्स का संग्रह दर्शाती है"
type: docs
weight: 1200
url: /hi/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

[`OutlineMask`](../outlinemask/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | इस संग्रह में निर्दिष्ट आइटम का सूचकांक निर्धारित करता है। |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | निर्दिष्ट सूचकांक पर निर्दिष्ट आइटम डालता है। |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | निर्दिष्ट सूचकांक पर एक आइटम हटाता है। |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


