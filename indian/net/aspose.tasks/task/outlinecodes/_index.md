---
title: "Task.OutlineCodes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। OutlineCodeCollection ऑब्जेक्ट प्राप्त करता है या सेट करता है"
type: docs
weight: 880
url: /hi/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

प्राप्त करता है या सेट करता है [`OutlineCodeCollection`](../../outlinecodecollection/) ऑब्जेक्ट।

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## टिप्पणियाँ

दो टुकड़े डेटा आवश्यक हैं - एक पॉइंटर जो outline code तालिका की ओर इशारा करता है जिसे FieldID द्वारा निर्दिष्ट किया गया है, और वह मान जो या तो ValueID या ValueGUID द्वारा निर्दिष्ट किया गया है, जो मान सूची की ओर पॉइंटर है।

## उदाहरण

टास्क के outline code मानों को पढ़ने का तरीका दिखाएँ।

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");
    var mapping = new Dictionary<string, OutlineValueCollection>();

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var code in project.OutlineCodes)
    {
        mapping.Add(code.FieldId, code.Values);
    }

    var task = project.RootTask.Children.GetById(2);
    foreach (var code in task.OutlineCodes)
    {
        var val = GetOutlineValue(mapping[code.FieldId], code.ValueId);
        Console.WriteLine("Outline value: " + val);
    }
}

public static object GetOutlineValue(OutlineValueCollection collection, int valueId)
{
    object obj = null;

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var value in collection)
    {
        if (value.ValueId != valueId)
        {
            continue;
        }

        obj = value.Value;
        break;
    }

    return obj;
}
```

### संबंधित देखें

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


