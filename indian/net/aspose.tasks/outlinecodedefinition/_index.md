---
title: "क्लास OutlineCodeDefinition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OutlineCodeDefinition क्लास। एक आउटलाइन कोड परिभाषा का प्रतिनिधित्व करता है।"
type: docs
weight: 1170
url: /hi/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

एक रूपरेखा कोड परिभाषा का प्रतिनिधित्व करता है।

```csharp
public sealed class OutlineCodeDefinition
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | `OutlineCodeDefinition` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | कस्टम आउटलाइन कोड का उपनाम प्राप्त करता है या सेट करता है। |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि नए कोडों में सभी स्तर होने चाहिए या नहीं। एंटरप्राइज़ कोड के लिए उपलब्ध नहीं है। |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं। |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | एक अन्य कस्टम फ़ील्ड का संदर्भ प्राप्त करता है या सेट करता है, जिसके लिए यह आउटलाइन कोड परिभाषा एक उपनाम है। |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | एक आउटलाइन कोड का फ़ील्ड नंबर प्राप्त करता है या सेट करता है। |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | कस्टम आउटलाइन कोड का नाम प्राप्त करता है या सेट करता है। |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | एक आउटलाइन कोड का Guid प्राप्त करता है या सेट करता है। |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मान लीफ़ वैल्यू होने चाहिए या नहीं। |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | OutlineMaskCollection ऑब्जेक्ट प्राप्त करता है। वह प्रविष्टियों की तालिका जो आउटलाइन कोड मास्क को परिभाषित करती है। केवल-पढ़ने योग्य [`OutlineMaskCollection`](../outlinemaskcollection/) उदाहरण। |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि निर्दिष्ट मान मान तालिका से होने चाहिए या नहीं। |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | कस्टम आउटलाइन कोड के उपनाम की ध्वन्यात्मक उच्चारण प्राप्त करता है या सेट करता है। |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि कस्टम आउटलाइन कोड को Microsoft Project में रिसोर्स सब्स्टीट्यूशन विज़ार्ड द्वारा उपयोग किया जा सकता है या नहीं। |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि इस आउटलाइन कोड के इंडेंट्स दिखाए जाने चाहिए या नहीं। |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | OutlineValueCollection ऑब्जेक्ट प्राप्त करता है। इस आउटलाइन कोड से जुड़ी तालिका के मान। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


