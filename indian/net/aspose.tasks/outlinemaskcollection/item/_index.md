---
title: "OutlineMaskCollection.Item"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineMaskCollection property. निर्दिष्ट इंडेक्स पर तत्व को लौटाता या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/outlinemaskcollection/item/
---
## OutlineMaskCollection indexer

निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है।

```csharp
public OutlineMask this[int index] { get; set; }
```

| पैरामीटर | विवरण |
| --- | --- |
| इंडेक्स | प्राप्त या सेट करने वाले तत्व का शून्य-आधारित अनुक्रमणिका। |

### रिटर्न वैल्यू

निर्दिष्ट अनुक्रमणिका पर तत्व।

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

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


