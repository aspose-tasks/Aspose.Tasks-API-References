---
title: "Prj.CurrencyCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। ISO 4217 में परिभाषित तीन अक्षर वाला मुद्रा कोड। वैध मानों का उदाहरण USD है।"
type: docs
weight: 150
url: /hi/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

ISO 4217 में परिभाषित तीन अक्षर वाला मुद्रा कोड। मान्य मानों का उदाहरण "USD" है।

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
```

## उदाहरण

दिखाता है कि परियोजना की मुद्रा प्रॉपर्टीज़ कैसे लिखें।

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// मुद्रा प्रॉपर्टीज़ सेट करें
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// मुद्रा प्रॉपर्टीज़ प्रदर्शित करें
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


