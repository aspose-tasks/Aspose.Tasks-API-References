---
title: "Prj.FiscalYearStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि वित्तीय वर्ष की क्रमांकन का उपयोग किया जाता है या नहीं"
type: docs
weight: 340
url: /hi/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

निर्धारित करता है कि वित्तीय वर्ष क्रमांकन उपयोग किया जाता है या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
```

## उदाहरण

दिखाता है कि वित्तीय वर्ष की प्रॉपर्टीज़ को कैसे लिखें।

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// वित्तीय वर्ष की गुणधर्म सेट करें
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// वित्तीय वर्ष की गुणधर्म दिखाएँ
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


