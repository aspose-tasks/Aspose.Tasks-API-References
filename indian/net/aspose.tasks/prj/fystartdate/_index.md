---
title: "Prj.FyStartDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj field. वह महीना जब वित्तीय वर्ष शुरू होता है"
type: docs
weight: 350
url: /hi/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

वित्तीय वर्ष के शुरू होने का महीना।

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
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
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


