---
title: "OutlineValue.ValueGuid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineValue प्रॉपर्टी। एक GUID प्राप्त करता है जो पूरे प्रोजेक्ट में अन्य मानों के बीच इस मान की पहचान करता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks/outlinevalue/valueguid/
---
## OutlineValue.ValueGuid property

एक GUID प्राप्त करता है जो पूरे प्रोजेक्ट में इस मान को अन्य मानों से पहचानता है।

```csharp
public Guid ValueGuid { get; }
```

## उदाहरण

रूपरेखा मानों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// एक रूपरेखा मान बनाएं
var value = new OutlineValue();

// वास्तविक मान सेट करें
value.Value = "Text value 1";

// परियोजना के भीतर रूपरेखा कोड मान की अद्वितीय आईडी सेट करें
value.ValueId = 1;

// पूरी परियोजना में इस मान को अन्य मानों से पहचानने वाला GUID प्राप्त करें
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// रूपरेखा कोड प्रकार सेट करें
value.Type = OutlineValueType.Text;

// रूपरेखा मान का विवरण सेट करें
value.Description = "Text value descr 1";

// रूपरेखा मान संकुचित है या नहीं, यह दर्शाने वाला मान सेट करें
value.IsCollapsed = false;

// पैरेंट मान आईडी जांचें
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// अवधि के साथ एक रूपरेखा मान बनाएं
var value2 = new OutlineValue();

// अवधि मान सेट करें
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// परियोजना के भीतर रूपरेखा कोड मान की अद्वितीय आईडी सेट करें
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### संबंधित देखें

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


