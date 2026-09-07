---
title: "एन्यूम CurrencySymbolPositionType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CurrencySymbolPositionType एन्यूम। मुद्रा प्रतीक की स्थिति को निर्दिष्ट करता है।"
type: docs
weight: 370
url: /hi/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

मुद्रा प्रतीक की स्थिति को निर्दिष्ट करता है।

```csharp
public enum CurrencySymbolPositionType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | संकेत करता है कि अपरिभाषित मान का अर्थ है कि फ़ील्ड मूल परियोजना फ़ाइल में परिभाषित नहीं था। |
| Before | `0` | पहले मुद्रा प्रतीक स्थिति प्रकार को दर्शाता है। |
| After | `1` | बाद में मुद्रा प्रतीक स्थिति प्रकार को दर्शाता है। |
| BeforeWithSpace | `2` | स्पेस के साथ पहले मुद्रा प्रतीक स्थिति प्रकार को दर्शाता है। |
| AfterWithSpace | `3` | स्पेस के साथ बाद में मुद्रा प्रतीक स्थिति प्रकार को दर्शाता है। |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

कैसे मुद्रा प्रतीक की स्थिति (CurrencySymbolPositionType.Before) निर्दिष्ट करें, दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");
// मुद्रा प्रतीक की स्थिति सेट करें
// पहले, कोई स्पेस नहीं ($0)।
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// परियोजना के साथ काम करें...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


