---
title: "OutlineCodeDefinition.ShowIndent"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineCodeDefinition प्रॉपर्टी। यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि इस आउटलाइन कोड के इंडेंट दिखाए जाने चाहिए या नहीं"
type: docs
weight: 140
url: /hi/net/aspose.tasks/outlinecodedefinition/showindent/
---
## OutlineCodeDefinition.ShowIndent property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि इस आउटलाइन कोड के इंडेंट्स दिखाए जाने चाहिए या नहीं।

```csharp
public bool ShowIndent { get; set; }
```

## टिप्पणियाँ

यह MS Project 2010 प्रॉपर्टी के लिए नया है।

## उदाहरण

आउटलाइन कोड परिभाषाओं के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// एक नया आउटलाइन कोड परिभाषा बनाएं
var outline = new OutlineCodeDefinition();

// एक आउटलाइन कोड का फ़ील्ड नंबर सेट करें
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// कस्टम आउटलाइन कोड का नाम सेट करें
outline.FieldName = "Outline Code1";

// एक आउटलाइन कोड का Guid सेट करें
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// एक मान सेट करें जो दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मान पत्ती मान होने चाहिए या नहीं
outline.LeafOnly = false;

// कस्टम आउटलाइन कोड का उपनाम सेट करें
outline.Alias = "My Outline Code";

// कस्टम आउटलाइन कोड के उपनाम की ध्वन्यात्मक उच्चारण सेट करें
outline.PhoneticAlias = "Outline Code";

// एक मान सेट करें जो दर्शाता है कि नए कोड को सभी स्तरों की आवश्यकता है या नहीं। एंटरप्राइज़ कोड के लिए उपलब्ध नहीं है।
outline.AllLevelsRequired = true;

// एक मान सेट करें जो दर्शाता है कि कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं
outline.Enterprise = false;

// एक अन्य कस्टम फ़ील्ड का संदर्भ सेट करें जिसके लिए यह आउटलाइन कोड परिभाषा उपनाम है
outline.EnterpriseOutlineCodeAlias = 0;

// एक आउटलाइन मास्क जोड़ें
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// एक मान सेट करें जो दर्शाता है कि निर्दिष्ट मान मान तालिका से आने चाहिए या नहीं
outline.OnlyTableValuesAllowed = false;

// एक मान सेट करें जो दर्शाता है कि कस्टम आउटलाइन कोड का उपयोग किया जा सकता है या नहीं
// Microsoft Project में रिसोर्स सब्स्टिट्यूशन विज़ार्ड द्वारा
outline.ResourceSubstitutionEnabled = false;

// एक मान सेट करें जो दर्शाता है कि इस आउटलाइन कोड के इंडेंट दिखाए जाने चाहिए या नहीं।
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### संबंधित देखें

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


