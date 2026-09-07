---
title: "Resource.OutlineCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource property. OutlineCodeCollection ऑब्जेक्ट प्राप्त करता है। एक outline code का मान"
type: docs
weight: 540
url: /hi/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

प्राप्त करता है एक OutlineCodeCollection ऑब्जेक्ट। एक रूपरेखा कोड का मान।

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## टिप्पणियाँ

दो टुकड़े डेटा आवश्यक हैं - एक पॉइंटर जो outline code तालिका की ओर इशारा करता है जिसे FieldID द्वारा निर्दिष्ट किया गया है, और वह मान जो या तो ValueID या ValueGUID द्वारा निर्दिष्ट किया गया है, जो मान सूची की ओर पॉइंटर है।

## उदाहरण

दिखाता है कि resource outline मानों के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### संबंधित देखें

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


